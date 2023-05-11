<template>
	<h2>About View</h2>
	{{ $route.path }}
	<button type="button" @click="$router.push('/')">Go to Home</button>
	<button type="button" @click="handleClickHome">Go to Home</button>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

const handleClickHome = () => {
	router.push('/');
};
</script>

<style lang="scss" scoped></style>
