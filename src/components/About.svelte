<script>
	export let buis, agencyName;
</script>

<section id="About" class="bg-white py-28 px-6 lg:px-20">
	<div id="FAQ" class="max-w-7xl mx-auto">
		<!-- Top Section: Image and Description -->
		<div class="lg:flex lg:items-center lg:space-x-12">
			<!-- Image -->
			<div class="flex-shrink-0 mb-8 lg:mb-0 lg:w-1/2">
				<img
					src={buis}
					alt="Team"
					class="rounded-lg shadow-lg lg:w-auto max-h-[500px] object-contain"
				/>
			</div>

			<!-- Description -->
			<div class="lg:w-1/2">
				<h2 class="text-3xl lg:text-4xl font-semibold mb-4 playfair">
					{agencyName}, <span class="text-primary">an OnlyFans and MYM agency</span> covering the full
					spectrum of account management
				</h2>
				<p class="text-gray-700 mb-4">
					{agencyName}, a French agency dedicated to OnlyFans and MYM account management, aims to
					optimize content creators' visibility and increase their earnings while ensuring their
					well-being and saving them valuable time.
				</p>
				<p class="text-gray-700">
					Our team of OnlyFans and MYM managers offers a range of services including account and
					social media management, development of a cohesive brand image, and advice and assistance
					on creative, legal, and financial aspects. We also ensure the protection of your content
					and take action against illegal sharing.
				</p>
			</div>
		</div>

		<!-- Values Section -->
		<div
			class="flex flex-col sm:flex-row justify-center items-center space-x-4 text-center my-10 sm:my-20 mx-2 playfair"
		>
			<div class="border-b-2 border-gray-300 flex-grow"></div>
			<span class="text-4xl sm:text-xl font-semibold">Humanity</span>
			<div class="border-b-2 border-gray-300 w-full my-3 sm:my-0 sm:w-auto flex-grow"></div>
			<span class="text-4xl sm:text-xl font-semibold">Trust</span>
			<div class="border-b-2 border-gray-300 w-full my-3 sm:my-0 sm:w-auto flex-grow"></div>
			<span class="text-4xl sm:text-xl font-semibold">Kindness</span>
			<div class="border-b-2 border-gray-300 w-full my-3 sm:my-0 sm:w-auto flex-grow"></div>
			<span class="text-4xl sm:text-xl font-semibold">Respect</span>
			<div class="border-b-2 border-gray-300 flex-grow"></div>
		</div>

		<!-- Call to Action Section -->
		<div
			class="bg-secondary text-white mt-12 p-8 rounded-lg shadow-lg flex flex-col lg:flex-row lg:items-center"
		>
			<div class="lg:w-2/3">
				<h3 class="text-2xl font-semibold mb-4">Why choose {agencyName}?</h3>
				<p class="text-lg mb-4">
					If you had to remember just one reason to work with us, we believe it would be this: {agencyName}
					is a truly human-centered agency. We treat our models as such, with respect and kindness. We
					are attentive to your well-being and fulfillment throughout our partnership. This is our core
					identity and our pride.
				</p>
				<p class="text-lg">
					Partner with {agencyName} and take your career to the next level without compromise.
				</p>
			</div>
			<div class="lg:w-1/3 mt-4 lg:mt-0 lg:pl-8 text-center lg:text-left">
				<a href="#hero" class="linkButtonPrimary hover:bg-tertiary hover:text-primary">
					Join {agencyName} →
				</a>
			</div>
		</div>
	</div>
</section>
