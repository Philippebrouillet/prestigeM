<script>
	import video from '$lib/vidéos/Video5.mp4';
	import { onMount } from 'svelte';
	export let agencyName;

	onMount(() => {
		document.addEventListener('DOMContentLoaded', function () {
			const video = document.getElementById('myVideo');
			video.play();
		});
	});
</script>

<main id="hero" class="relative h-screen flex justify-center items-center overflow-hidden">
	<!-- Background Video -->
	<video
		id="myVideo"
		src={video}
		autoplay
		muted
		loop
		playsinline
		preload="auto"
		class="absolute top-0 left-0 w-full h-full object-cover z-0"
	>
	</video>

	<!-- Content on top of the video -->
	<div class="relative text-center py-20 px-4 text-white max-w-2xl lg:max-w-4xl z-10 mt-10">
		<h1 class="text-3xl lg:text-4xl font-semibold mb-10 playfair leading-10 tracking-wide">
			Boost your <span class="text-tertiary text-highlight">OnlyFans</span> and
			<span class="text-tertiary text-highlight">MYM</span>
			earnings with the management agency {agencyName}
		</h1>
		<div class="flex justify-center mb-10">
			<p class="lg:text-lg w-full max-w-xl font-medium">
				{agencyName} helps content creators reach the Top 1% on OnlyFans and MYM to maximize their earnings
			</p>
		</div>
		<div class="flex flex-col md:flex-row gap-4 md:gap-6 justify-center">
			<a href="#Contact" class="linkButtonPrimary border-2 border-primary hover:border-secondary"
				>Join {agencyName}</a
			>
			<a
				href="#About"
				class="linkButtonPrimary bg-transparent border-2 border-gray-300 text-gray-300 hover:bg-transparent hover:border-opacity-80 hover:text-tertiary"
			>
				Learn more
			</a>
		</div>
	</div>

	<!-- Optional overlay to darken the video -->
	<div class="absolute top-0 left-0 w-full h-full bg-black opacity-50 z-5"></div>
</main>

<style>
	.text-highlight {
		color: #ffe4e4ec;
		text-shadow: 2px 2px 6px #c6605d;
		font-weight: bold;
		border-radius: 5px;
	}
</style>
