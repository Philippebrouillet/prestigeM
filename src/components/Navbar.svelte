<script>
	import logo from '$lib/images/logo.png';
	import { scale } from 'svelte/transition';

	let scrollY;
	let innerWidth;
	let openMobilMenu = false;

	const toggleMobilMenu = () => {
		openMobilMenu = !openMobilMenu;
	};

	const scrollLimit = 100;
	const links = ['Solutions', 'Results', 'Services', logo, 'About', 'FAQ', 'Contact'];
</script>

<svelte:window bind:scrollY bind:innerWidth />

{#if innerWidth > 1000}
	<header
		class=" transition-all duration-300 {scrollY > scrollLimit
			? ' bg-gradient-to-t from-primary/70 via-secondary/90 to-tertiary/95 text-white'
			: 'bg-transparent text-white'} z-50 fixed top-0 w-full flex justify-center items-center"
	>
		<nav class="transition-all duration-300 {scrollY > scrollLimit ? 'py-4' : 'py-5'}">
			<ul class:text-lg={scrollY < scrollLimit} class="flex justify-center items-center gap-6">
				{#each links as link, i}
					{#if i === 3}
						<li>
							<a href="#hero">
								<img
									src={link}
									alt="logo"
									class="transition-all duration-200 shadow-lg shadow-primary/20 {scrollY >
									scrollLimit
										? ' h-12 border-2 border-white'
										: ' h-16 '}    cursor-pointer rounded-full"
								/>
							</a>
						</li>
					{:else}
						<li>
							<a href="#{link}" class="navlink">{link}</a>
						</li>
					{/if}
				{/each}
			</ul>
		</nav>
	</header>
{:else}
	<header
		class=" transition-all duration-300 {scrollY > scrollLimit
			? ' bg-gradient-to-t from-primary/70 via-secondary/90 to-tertiary/95 text-white'
			: 'bg-transparent text-white'} z-50 fixed top-0 w-full flex justify-center items-center"
	>
		<nav
			class="transition-all duration-300 w-full max-w-2xl mx-6 flex justify-between {scrollY >
			scrollLimit
				? 'py-3'
				: 'py-5'}"
		>
			<a href="#hero">
				<img
					src={logo}
					alt="logo"
					class="transition-all duration-200 shadow-lg shadow-primary/20 {scrollY > scrollLimit
						? ' h-12 border-2 border-white'
						: ' h-16'}    cursor-pointer rounded-full"
				/>
			</a>

			<button on:click={toggleMobilMenu}
				><svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="2"
					stroke="currentColor"
					class="w-8 h-8"
				>
					<path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16m-7 6h7" />
				</svg></button
			>
		</nav>
	</header>

	{#if openMobilMenu}
		<div
			class="fixed z-[100] top-0 left-0 w-screen h-screen bg-tertiary flex justify-center items-center"
		>
			<button class="fixed top-10 right-10 z-[400] text-primary" on:click={toggleMobilMenu}
				><svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="2"
					stroke="currentColor"
					class="w-8 h-8"
				>
					<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
				</svg></button
			>
			<ul
				class="flex max-h-screen overflow-y-auto flex-col justify-start items-center gap-5 text-white text-3xl"
			>
				<a on:click={toggleMobilMenu} href="#hero">
					<img
						src={logo}
						alt="logo"
						class="transition-all text-left shadow-lg shadow-primary/20 border-2 border-white duration-200 h-28 cursor-pointer rounded-full mb-10"
					/>
				</a>
				{#each links as link, i}
					{#if i === 3}
						<div class="hidden"></div>
					{:else}
						<li>
							<a on:click={toggleMobilMenu} href="#{link}" class="navlink">{link}</a>
						</li>
					{/if}
				{/each}
			</ul>
		</div>
	{/if}
{/if}

{#if scrollY > scrollLimit}
	<a
		in:scale
		href="#hero"
		class="fixed bottom-6 border border-white right-6 z-50 bg-primary text-white p-2.5 rounded-full shadow-lg hover:bg-secondary transition transform hover:-translate-y-1 hover:shadow-xl"
		aria-label="Back to Top"
	>
		<svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="h-6 w-6" viewBox="0 0 20 20">
			<path
				fill-rule="evenodd"
				d="M3.293 12.707a1 1 0 011.414 0L10 7.414l5.293 5.293a1 1 0 001.414-1.414l-6-6a1 1 0 00-1.414 0l-6 6a1 1 0 001.414 1.414z"
				clip-rule="evenodd"
			/>
		</svg>
	</a>
{/if}
