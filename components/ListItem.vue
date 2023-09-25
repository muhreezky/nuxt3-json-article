<template>
	<nuxt-link :to="`/${$props.articleId}`">
		<div class="mx-2 border-2 border-black rounded-lg p-5 flex flex-col gap-3">
			<div>
				<b>ID : </b>{{ $props.articleId }}
			</div>
			<div>
				<b>Title : </b> {{ $props.articleTitle }}
			</div>
		</div>
	</nuxt-link>
</template>

<script lang="ts" setup>
	defineProps(['articleId', 'articleTitle']);
</script>