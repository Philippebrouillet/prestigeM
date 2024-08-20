<script>
	export let agencyName, unique, gestion, vente, formation, planification, assistance;
</script>

<section id="Services" class="py-28 px-6 lg:px-20 border-y border-primary bg-secondary/20">
	<div class="max-w-7xl mx-auto text-center mb-12">
		<!-- Section Title -->
		<h2 class="text-3xl lg:text-4xl font-semibold mb-4 playfair">
			<span class="text-primary">A tailored strategy and support</span>
			<br />
			to stand out on OnlyFans and MYM
		</h2>
		<div class="flex justify-center">
			<p class="lg:text-lg text-gray-700 max-w-2xl">
				As an OnlyFans and MYM agency, {agencyName} offers personalized support and services tailored
				to each model. Our specialized managers continuously monitor your account and adjust actions
				to ensure optimal performance.
			</p>
		</div>
	</div>
	<div class="flex justify-center items-center w-full">
		<!-- Services Grid -->
		<div class="grid grid-cols-1 lg:grid-cols-2 xl:grid-cols-3 gap-8 max-w-6xl">
			<!-- Card 1 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<img class="h-8 w-8" src={unique} alt="unique" />
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Defining Your Unique Image</h3>
				<p>
					If you have not yet established a clear positioning and distinct image, our mission is to
					define them together. A striking, unique, and engaging identity is essential to
					differentiate yourself and attract sales. It is your digital value, the foundation of your
					success, and the cornerstone of your content strategy to better target your audience or a
					specific niche.
				</p>
			</div>

			<!-- Card 2 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<img class="h-8 w-8 whiteImg" src={gestion} alt="management" />
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">MYM and OnlyFans Account Management</h3>
				<p>
					Focus on creation, and we'll handle the rest! Our OnlyFans and MYM managers guide you on
					the type of content to create to maximize your results. We manage your social media
					distribution, prepare your videos, and craft effective and optimized captions. This
					virtuous cycle will drive your success!
				</p>
			</div>

			<!-- Card 3 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<img class="h-8 w-8 whiteImg" src={vente} alt="marketing" />
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Marketing and Promotion</h3>
				<p>
					Followers, conversion to paying subscribers, revenue—everything starts with your
					visibility. We implement online actions to highlight your platforms, creators, and
					increase your traffic. Through various free and paid communication channels, we bring new
					fans to discover you every day.
				</p>
			</div>

			<!-- Card 4 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<img class="h-8 w-8 whiteImg" src={formation} alt="training" />
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Advice, Support, and Training</h3>
				<p>
					We take pride in supporting our models on their journey to success by offering
					personalized service. Our caring approach includes advice on presentation, relationships,
					and monetization of your fan base. You are guided toward success, benefiting from the
					expertise of dedicated coaches committed to your growth.
				</p>
			</div>

			<!-- Card 5 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<img class="h-8 w-8 whiteImg" src={planification} alt="planning" />
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Planning and Inspiration</h3>
				<p>
					To help you overcome potential creative blocks or motivation lapses, we continuously
					monitor trends. We provide inspiring content ideas along with the schedule for your posts.
					These ideas are then brought to life with creative visuals and concepts. Strengthen your
					presence to stand out.
				</p>
			</div>

			<!-- Card 6 -->
			<div
				id="Contact"
				class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary"
			>
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<img class="h-8 w-8 whiteImg" src={assistance} alt="assistance" />
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Assistance and Support</h3>
				<p>
					Receive comprehensive assistance for managing your OnlyFans and MYM accounts. The agency
					handles technical issues, performance analysis, legal aspects, and marketing. We ensure
					your rights are protected, securing your content. Assistance Solutions are at your
					disposal to address any problem and give you peace of mind.
				</p>
			</div>
		</div>
	</div>

	<!-- Call to Action -->
	<div class="mt-12 text-center flex justify-center">
		<a href="#hero" class="linkButtonPrimary"> Join {agencyName} </a>
	</div>
</section>
