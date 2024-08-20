<script>
	import { slide } from 'svelte/transition';
	export let agencyName, email;
	let faqs = [
		{
			question: 'What are OnlyFans and MYM? How do they work?',
			answer:
				'OnlyFans and MYM are platforms aimed at establishing and maintaining a privileged relationship between content creators and their fans. Fans can subscribe to monthly subscriptions typically ranging from $4.99 to $49.99 to access exclusive content, such as videos, photos, and private messages. Fans can also tip in exchange for personalized dedications or content. Content creators generally invite their subscribers to join them on OnlyFans or MYM from other mainstream sites or social networks, such as Twitter, Instagram, TikTok, YouTube, or Twitch. As of early 2023, OnlyFans has over 190 million users, and MYM, which focuses on the French market, has over 10 million. Many public figures now use OnlyFans and MYM to maintain privileged relationships with their audience and build fan loyalty through unique, high-quality content.'
		},
		{
			question: 'Are these platforms legal?',
			answer:
				"Users (creators and fans) must be at least 18 years old and exclude anyone under this age from their content. They are also required to use their accounts for legal purposes. The terms of service for OnlyFans and MYM explicitly specify what is allowed and what is not. Any adult with a bank account can create a 'creator' account on these platforms and charge for access to their content."
		},
		{
			question: 'What is the average income of content creators on OnlyFans and MYM?',
			answer:
				'On OnlyFans, creators typically have 21 fans and earn between $140 and $180 per month. The top 1% of creators capture 33% of all earnings, and the top 10% take 73%. Achieving these results requires a strategy and almost constant content publishing. As such, most top creators are represented by OnlyFans and MYM management agencies. (MYM does not disclose average earnings of its creators, but testimonies suggest that the figures are similar.)'
		},
		{
			question: 'How long does it take to get paid on MYM and OnlyFans?',
			answer:
				'After you make your first earnings (subscriptions or tips) via OnlyFans or MYM, your first payout will be initiated and should be finalized within 7 to 10 days. Note that this refers to 7 to 10 days after your first receipt of funds, not after the creation of your account. The exact date of your first payment may vary depending on various factors.'
		},
		{
			question: 'What is an OnlyFans and MYM account management agency?',
			answer:
				'An OnlyFans and MYM account management agency consists of managers dedicated to promoting and developing OnlyFans and MYM accounts for content creators. The agency implements a set of strategies and tactics, such as content optimization, social media marketing, influencer collaborations, and paid marketing, to increase the number of subscribers, engagement, and revenue generated.'
		},
		{
			question: `How can ${agencyName} help me grow and increase my revenue on OnlyFans and/or MYM?`,
			answer: `The ${agencyName} team works closely with you to design and implement a comprehensive and personalized marketing strategy that meets your goals and target audience. Beyond advice and support, the agency handles account management, the development and optimization of content strategies, social media marketing, influencer collaborations, paid marketing, as well as analysis and performance tracking.`
		},
		{
			question: `Do I really need an agency? Why should I choose ${agencyName} instead of doing everything myself?`,
			answer: `It is entirely possible to promote and manage your OnlyFans or MYM by yourself. However, to be successful, it requires continuous strategy implementation and management: "It's not a new gold mine at all. You have to do photo shoots, invest in social media to promote your page, respond to custom requests... it's a huge investment, with returns that are far from guaranteed. To earn even a minimum wage, you have to spend all day on it." – Noémie, 25 years old (interview in Le Monde). Working with ${agencyName} allows you to benefit from our team's expertise in this industry and increase your earnings to levels far beyond what you could achieve alone. Moreover, not only will your earnings increase, but your time will too, as you will only need to focus on the creative aspect, while the agency takes care of everything else. Therefore, choosing ${agencyName} is a wise choice for creators who want to focus on their content, their time, and experience real growth.`
		}
	];

	function toggleFaq(index) {
		faqs = faqs.map((faq, i) => {
			if (i === index) {
				faq.open = !faq.open;
			} else {
				faq.open = false;
			}
			return faq;
		});
	}
</script>

<div id="FAQ" class="max-w-7xl mx-auto p-6 pb-28 flex flex-col lg:flex-row gap-10">
	<div class="lg:w-2/5">
		<h2 class="text-3xl font-semibold text-gray-900 mb-6 playfair">
			Frequently Asked Questions (FAQ)
		</h2>
		<p class="text-gray-500">
			You have questions, and that’s perfectly normal. We aim to answer as many as possible in the
			following FAQ. If some are not covered here, <a
				href={`mailto:${email}`}
				class="underline hover:text-primary">feel free to send us a message.</a
			>
		</p>
	</div>
	<div class="grid grid-cols-1 gap-5 w-full">
		{#each faqs as faq, index}
			<div class="border-b border-gray-300 py-6">
				<button
					on:click={() => toggleFaq(index)}
					class="w-full text-left flex justify-between items-center text-gray-700 font-semibold text-lg"
				>
					{faq.question}
					<svg
						class="min-w-5 min-h-5 w-5 h-5 transform transition-transform duration-200"
						class:rotate-180={faq.open}
						fill="none"
						stroke="currentColor"
						viewBox="0 0 24 24"
						xmlns="http://www.w3.org/2000/svg"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M19 9l-7 7-7-7"
						/>
					</svg>
				</button>
				{#if faq.open}
					<p in:slide class="mt-4 text-gray-600">{faq.answer}</p>
				{/if}
			</div>
		{/each}
	</div>
</div>

<style>
	button {
		outline: none;
	}
</style>
