<script lang="ts">
	import TopicCard from '$lib/components/TopicCard.svelte';
	import TopicList from '$lib/components/TopicList.svelte';

	function scrollToSection() {
		const targetSection = document.querySelector('#target-section');
		if (targetSection) {
			targetSection.scrollIntoView({ behavior: 'smooth' });
		}
	}
</script>

<div class="hero min-h-screen bg-base-200">
	<div class="hero-content text-center">
		<div class="max-w-md">
			<h1 class="text-5xl font-bold">Hello there</h1>
			<p class="py-6">
				Wellcome in the Secure Coding Cookbook site where you can read a bunch of information about
				secure coding.
			</p>
			<button class="btn btn-outline btn-info" on:click={scrollToSection}>Info</button>
		</div>
	</div>
</div>

<section id="target-section" class="">
	<TopicList />
</section>
