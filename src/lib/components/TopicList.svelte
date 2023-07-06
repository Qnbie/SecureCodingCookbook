<script lang="ts">
	import { onMount } from 'svelte';
	import TopicCard from './TopicCard.svelte';

	let topics: any[] = [];

	onMount(async () => {
		const response = await fetch(`/topics.json`);
		topics = await response.json();
	});
</script>

{#each topics as topic}
	<TopicCard>
		<span slot="title">{topic.title}</span>
		<span slot="description">{topic.description}</span>
		<a class="btn btn-outline" slot="button" href={topic.url}>Button to the topic</a>
	</TopicCard>
{/each}
