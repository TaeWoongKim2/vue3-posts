<template>
	<h2>Home View</h2>
	{{ $route.path }}
	<button type="button" class="btn btn-primary" @click="$router.push('/about')">
		Go to About
	</button>
	<button type="button" class="btn btn-primary" @click="handleClickAbout">
		Go to About
	</button>
</template>

<script setup>
import { useRoute, useRouter } from 'vue-router';

const route = useRoute();
console.log('[route.path]:', route.path);

const router = useRouter();

const handleClickAbout = () => {
	router.push('/about');
};
</script>

<style lang="scss" scoped></style>
