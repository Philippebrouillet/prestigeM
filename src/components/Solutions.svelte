<script>
	export let agencyName, argent, timeplus, perso;
</script>

<section id="Solutions" class="py-28 px-6 lg:px-20 border-y border-primary bg-secondary/20">
	<div class="max-w-7xl mx-auto text-center mb-12">
		<!-- Heading -->
		<h2 class="text-3xl lg:text-4xl font-semibold mb-10 playfair">
			With the {agencyName} agency, multiply your earnings
			<br />
			and <span class="text-primary">aim for the top 1% of MYM and OnlyFans</span>
		</h2>
		<div class="flex justify-center">
			<p class="lg:text-lg text-gray-700 max-w-2xl">
				The managers at {agencyName} specialize in managing OnlyFans and MYM accounts. They assist models
				and content creators in boosting their earnings and freeing up their time by handling all the
				management tasks. You regain your free time while improving your performance!
			</p>
		</div>
	</div>

	<!-- Cards Section -->
	<div class="flex flex-col lg:flex-row gap-8 justify-center">
		<!-- Card 1 -->
		<div
			class="bg-white border-t-2 border-primary p-8 rounded-lg shadow-lg flex flex-col items-start text-left text-white"
		>
			<div class="mb-4">
				<!-- Icon (You can replace with appropriate SVG) -->
				<div class="bg-tertiary text-white p-3 rounded-full">
					<img class="h-8 w-8" src={argent} alt="money" />
				</div>
			</div>
			<h3 class="text-xl font-semibold mb-2 text-gray-800 playfair h-[70px]">
				Boost Your MYM and OnlyFans Earnings
			</h3>
			<p class="text-gray-400 text-sm playfair">
				{agencyName} enhances your earnings on MYM and OnlyFans through proven expertise and strategies
				in marketing and positioning. By optimizing your image and content, we maximize your profits
				without compromising your values. Together, we turn your talent into financial success.
			</p>
		</div>

		<!-- Card 2 -->
		<div
			class="bg-white p-8 border-t-2 border-primary rounded-lg shadow-lg flex flex-col items-start text-left text-white"
		>
			<div class="mb-4">
				<!-- Icon (You can replace with appropriate SVG) -->
				<div class="bg-tertiary text-white p-3 rounded-full">
					<img class="h-8 w-8" src={timeplus} alt="time" />
				</div>
			</div>
			<h3 class="text-xl font-semibold mb-2 text-gray-800 playfair h-[70px]">Save Time</h3>
			<p class="text-gray-400 text-sm playfair">
				By managing your OnlyFans and MYM accounts for you, {agencyName} frees up your schedule. Our
				experts take care of your social media, writing, and posts, allowing you to focus on what matters.
				More time also means more opportunities to express your talent!
			</p>
		</div>

		<!-- Card 3 -->
		<div
			class="bg-white p-8 border-t-2 border-primary rounded-lg shadow-lg flex flex-col items-start text-left text-primary"
		>
			<div class="mb-4">
				<!-- Icon (You can replace with appropriate SVG) -->
				<div class="bg-tertiary text-white p-3 rounded-full">
					<img class="h-8 w-8" src={perso} alt="personalized" />
				</div>
			</div>
			<h3 class="text-xl font-semibold mb-2 text-gray-800 playfair h-[70px]">
				Enjoy Personalized Support
			</h3>
			<p class="text-gray-400 text-sm playfair">
				Because you are unique, we offer unique support. Together, we define your image, your
				differences, and a tailor-made strategy. Our team is attentive, responsive, and deeply
				concerned with your growth and success. Beyond success, we aim for your fulfillment and a
				long-lasting partnership.
			</p>
		</div>
	</div>
</section>
