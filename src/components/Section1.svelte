<script>
	export let girl, concu, marketing, motivation;
</script>

<section class="bg-white py-28 px-6 lg:px-20">
	<div class="max-w-7xl mx-auto">
		<!-- Section Heading -->
		<div class="text-center mb-12">
			<h2 class="text-3xl lg:text-4xl font-semibold playfair mb-10">
				Succeeding on OnlyFans and MYM is <span class="text-primary">not that easy...</span>
			</h2>

			<div class="flex justify-center">
				<p class="lg:text-lg text-gray-700 max-w-2xl">
					While it's easy to start creating content on OnlyFans and MYM with dreams of earning 5 or
					6 figures monthly, the reality is quite different. Competition is fierce, obstacles are
					numerous, and starting without external help often leads to disillusionment!
				</p>
			</div>
		</div>

		<!-- Section Content -->
		<div class="flex flex-col lg:flex-row items-start gap-8">
			<!-- Left Column with Image -->
			<div class="w-full lg:w-1/3">
				<img
					src={girl}
					alt="Illustration"
					class="rounded-lg shadow-lg max-h-[500px] w-full sm:w-auto lg:max-h-[2000px] object-cover"
				/>
			</div>

			<!-- Right Column with Text Content -->
			<div class="w-full lg:w-2/3 grid grid-cols-1 lg:grid-cols-2 gap-8 mt-4">
				<!-- Card 1 -->
				<div class="flex flex-col gap-3">
					<div class="bg-primary w-[57px] text-white p-3 rounded-full">
						<img class="h-8 w-8 whiteImg" src={concu} alt="competition" />
					</div>

					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">A lot of competition</h3>
						<p class="mt-4 text-gray-400 text-sm">
							In 2023, MYM has 150,000 creators, and OnlyFans 2.1 million. The average earnings on
							OnlyFans are $150/month, while the top 1% alone captures 73% of the revenue! Standing
							out is not easy!
						</p>
					</div>
				</div>

				<!-- Card 2 -->
				<div class="flex flex-col gap-3">
					<div class="bg-primary text-white w-[57px] p-3 rounded-full">
						<img class="h-8 w-8 whiteImg" src={marketing} alt="marketing" />
					</div>

					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">No marketing strategy</h3>
						<p class="mt-4 text-gray-400 text-sm">
							Posting content without a clear direction, differentiated strategy, or marketing
							optimization almost always leads to disappointing results. Unfortunately, this is the
							case for most creators on OnlyFans and MYM.
						</p>
					</div>
				</div>

				<!-- Card 3 -->
				<div class="flex flex-col gap-3">
					<div class="bg-primary w-[57px] text-white p-3 rounded-full">
						<img class="h-8 w-8 whiteImg" src={motivation} alt="motivation" />
					</div>
					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">
							Lack of discipline and motivation
						</h3>
						<p class="mt-4 text-gray-400 text-sm">
							Success on OnlyFans and MYM requires persistence and motivation over the long term.
							Sticking to the pace alone over time is a challenge. Many creators end up giving up!
						</p>
					</div>
				</div>

				<!-- Card 4 -->
				<div class="flex flex-col gap-3">
					<div class="bg-primary w-[57px] text-white p-3 rounded-full">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
							stroke-width="2"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M12 6v6l4 2M12 2a10 10 0 0110 10 10 10 0 01-10 10 10 10 0 01-10-10A10 10 0 0112 2z"
							/>
						</svg>
					</div>

					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">Lack of time</h3>
						<p class="mt-4 text-gray-400 text-sm">
							Managing OnlyFans and MYM accounts requires constant attention. Creating content,
							writing captions, responding to messages, promoting on social media... succeeding in
							this field is extremely time-consuming!
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
