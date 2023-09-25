<template>
	<div className="flex flex-col gap-4">
		<list-item
			v-for="(article, key) in articles"
			:key="key"
			:articleTitle="article.title"
			:articleId="article.id as string"
		/>
	</div>
</template>

<script lang="ts" setup>
import { articles } from "~/data/articles.json";
</script>
