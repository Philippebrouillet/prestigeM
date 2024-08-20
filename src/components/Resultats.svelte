<script>
	export let agencyName, result1, result2;
</script>

<section id="Results" class="bg-white py-28 px-6 lg:px-20">
	<div class="max-w-7xl mx-auto">
		<!-- Section Header -->

		<!-- Result Cards -->

		<div class="mb-14">
			<h2 class="text-3xl font-semibold mb-4 playfair">
				<span class="text-primary">Recent Results</span> of {agencyName} Agency Models on OnlyFans and
				MYM
			</h2>
			<p class="text-lg text-gray-700">
				Here are the results and earnings you can achieve by joining {agencyName} Agency.
			</p>
			<a href="#hero" class="text-primary font-semibold mt-2 inline-block"
				>Find out how to achieve these results →</a
			>
		</div>
		<div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
			<!-- Card 1 -->
			<img src={result1} alt="Chart 1" class="w-full object-cover rounded-md max-h-[600px]" />

			<!-- Card 2 -->
			<img src={result2} alt="Chart 2" class="w-full object-cover rounded-md max-h-[600px]" />
		</div>
	</div>
</section>
