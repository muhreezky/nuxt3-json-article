<template>
	<header>
		<h1 class="text-3xl font-extrabold">
			{{ article.title }}
		</h1>
	</header>
	<main class="flex gap-3 flex-col">
		<img :src="article.img" :alt="title" class="max-w-full" />
		<div class="content">
			{{ article.content }}
		</div>
	</main>
</template>

<script setup>
	import { articles } from "~/data/articles.json";
	const route = useRoute();
	const article = articles.filter(({ id }) => id === route.params.articleId)[0];
</script>