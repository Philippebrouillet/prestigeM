<script>
	import '../app.css';
	import logo from '$lib/images/logo.png';

	import girl1 from '$lib/images/girl1.png';
	import buis from '$lib/images/buis.png';
	import Navbar from '../components/Navbar.svelte';
	const agencyName = 'Mia Prestige';

	let videoUrl =
		'https://honeyfans-agency.com/wp-content/uploads/2023/07/video-header-HoneyFans-Agency-v3-720p.mp4';
</script>

<svelte:head>
	<title>{agencyName}</title>
	<meta name="description" content={agencyName} />
</svelte:head>

<Navbar />

<!-- HERO SECTION  -->
<main id="hero" class="relative h-screen flex justify-center items-center overflow-hidden">
	<!-- Background Video -->
	<video
		src={videoUrl}
		autoplay
		muted
		loop
		playsinline
		class="absolute top-0 left-0 w-full h-full object-cover z-0"
	>
	</video>

	<!-- Content on top of the video -->
	<div class="relative text-center py-20 px-4 text-white max-w-2xl lg:max-w-4xl z-10">
		<h1 class="text-3xl lg:text-4xl font-semibold mb-10 playfair leading-10">
			Boostez vos revenus OnlyFans et MYM grâce à l’agence de management {agencyName}
		</h1>
		<div class="flex justify-center mb-10">
			<p class="lg:text-lg w-full max-w-xl font-semibold">
				{agencyName} aide les créatrices de contenu à rentrer dans le Top 1% sur OnlyFans et MYM pour
				maximiser leurs revenus
			</p>
		</div>
		<div class="flex justify-center space-x-4">
			<a href="#hero" class="linkButtonPrimary">Rejoignez {agencyName}</a>
			<a
				href="#hero"
				class="bg-gray-800 flex justify-center items-center text-white py-2 px-6 rounded-lg font-semibold transition-colors duration-200 hover:bg-gray-700"
			>
				En savoir plus
			</a>
		</div>
	</div>

	<!-- Optional overlay to darken the video -->
	<div class="absolute top-0 left-0 w-full h-full bg-black opacity-50 z-5"></div>
</main>

<!-- SECTION 1  -->
<section class="bg-white py-28 px-6 lg:px-20">
	<div class="max-w-7xl mx-auto">
		<!-- Section Heading -->
		<div class="text-center mb-12">
			<h2 class="text-3xl lg:text-4xl font-semibold playfair mb-10">
				Réussir sur OnlyFans et MYM, ce n’est <span class="text-primary">pas si facile...</span>
			</h2>

			<div class="flex justify-center">
				<p class=" lg:text-lg text-gray-700 max-w-2xl">
					S'il est facile de se lancer dans la création de contenu sur OnlyFans et MYM avec des
					rêves de revenus mensuels à 5 ou 6 chiffres, la réalité est tout autre. La concurrence est
					rude, les obstacles nombreux et se lancer sans aide extérieure conduit souvent à des
					désillusions !
				</p>
			</div>
		</div>

		<!-- Section Content -->
		<div class="flex flex-col lg:flex-row items-start gap-8">
			<!-- Left Column with Image -->
			<div class="w-full lg:w-1/3">
				<img src={girl1} alt="Illustration" class="rounded-lg shadow-lg" />
			</div>

			<!-- Right Column with Text Content -->
			<div class="w-full lg:w-2/3 grid grid-cols-1 lg:grid-cols-2 gap-8">
				<!-- Card 1 -->
				<div class="flex flex-col gap-2">
					<div class="bg-primary w-[57px] text-white p-3 rounded-full">
						<!-- Replace with an appropriate icon -->
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
							stroke-width="2"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M8 9l4-4 4 4m0 6l-4 4-4-4" />
						</svg>
					</div>

					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">Beaucoup de concurrence</h3>
						<p class="mt-2 text-gray-400 text-sm">
							En 2023, MYM compte 150 000 créatrices et créateurs, OnlyFans 2,1 millions. La moyenne
							des gains sur OnlyFans est de $150/mois, alors que le Top 1% capte à lui seul 73% des
							revenus! Se démarquer ne s'improvise pas !
						</p>
					</div>
				</div>

				<!-- Card 2 -->
				<div class="flex flex-col gap-2">
					<div class="bg-primary text-white w-[57px] p-3 rounded-full">
						<!-- Replace with an appropriate icon -->
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
							stroke-width="2"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M3 3h18v18H3V3z" />
						</svg>
					</div>

					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">Pas de stratégie marketing</h3>
						<p class="mt-2 text-gray-400 text-sm">
							Poster du contenu sans ligne directrice, stratégie différenciatrice ou optimisation
							marketing conduit presque toujours à des résultats décevants. C'est malheureusement le
							cas d'une majorité de créateurs sur OnlyFans et MYM.
						</p>
					</div>
				</div>

				<!-- Card 3 -->
				<div class="flex flex-col gap-2">
					<div class="bg-primary w-[57px] text-white p-3 rounded-full">
						<!-- Replace with an appropriate icon -->
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
							stroke-width="2"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M12 8v8m4-4H8" />
						</svg>
					</div>
					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">
							Manque de rigueur et motivation
						</h3>
						<p class="mt-2 text-gray-400 text-sm">
							Le succès sur OnlyFans et MYM requiert assiduité et motivation sur le long terme.
							S'accrocher et tenir le rythme seul.e dans la durée est un défi. Nombreux sont les
							créateurs qui finissent par abandonner !
						</p>
					</div>
				</div>

				<!-- Card 4 -->
				<div class="flex flex-col gap-2">
					<div class="bg-primary w-[57px] text-white p-3 rounded-full">
						<!-- Replace with an appropriate icon -->
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-8 w-8"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
							stroke-width="2"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4m0 4h.01" />
						</svg>
					</div>

					<div>
						<h3 class="text-xl font-semibold text-gray-700 playfair">Manque de temps</h3>
						<p class="mt-2 text-gray-400 text-sm">
							Créer des comptes OnlyFans et MYM demande une attention constante. Créer du contenu,
							rédiger les légendes, répondre aux messages, promouvoir sur les réseaux sociaux...
							réussir dans ce domaine est terriblement chronophage !
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- SECTION SOLUTION  -->

<section id="Solution" class="bg-white py-28 px-6 lg:px-20 border-y border-primary bg-primary/10">
	<div class="max-w-7xl mx-auto text-center mb-12">
		<!-- Heading -->
		<h2 class="text-3xl lg:text-4xl font-semibold mb-10 playfair">
			Avec l'agence {agencyName}, multipliez vos revenus
			<br />
			et <span class="text-primary">visez le top 1% de MYM et Onlyfans</span>
		</h2>
		<div class="flex justify-center">
			<p class=" lg:text-lg text-gray-700 max-w-2xl">
				Les managers et manageuses de l'agence {agencyName} se spécialisent en management de comptes
				OnlyFans et MYM. Ils accompagnent les modèles et créatrices de contenu pour booster leurs revenus
				et libérer leur temps en s'occupant de toute la partie gestion. Vous retrouvez votre temps libre,
				tout en gagnant en performance !
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
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="2"
						stroke="currentColor"
						class="h-8 w-8"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M12 8v4m0 4h.01M12 8v4m0 4h.01M12 8v4m0 4h.01"
						/>
					</svg>
				</div>
			</div>
			<h3 class="text-xl font-semibold mb-2 text-gray-800 playfair h-[70px]">
				Boostez vos revenus MYM et OnlyFans
			</h3>
			<p class="text-gray-400 text-sm playfair">
				{agencyName} booste vos revenus sur MYM et OnlyFans par une expertise et des stratégies éprouvées
				en marketing et positionnement. En optimisant votre image et votre contenu, nous maximisons vos
				gains sans compromettre vos valeurs. Ensemble, nous transformons votre talent en succès financier.
			</p>
		</div>

		<!-- Card 2 -->
		<div
			class="bg-white p-8 border-t-2 border-primary rounded-lg shadow-lg flex flex-col items-start text-left text-white"
		>
			<div class="mb-4">
				<!-- Icon (You can replace with appropriate SVG) -->
				<div class="bg-tertiary text-white p-3 rounded-full">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="2"
						stroke="currentColor"
						class="h-8 w-8"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M12 8v4m0 4h.01M12 8v4m0 4h.01M12 8v4m0 4h.01"
						/>
					</svg>
				</div>
			</div>
			<h3 class="text-xl font-semibold mb-2 text-gray-800 playfair h-[70px]">Gagnez du temps</h3>
			<p class="text-gray-400 text-sm playfair">
				En gérant vos comptes OnlyFans et MYM pour vous, {agencyName} libère votre emploi du temps. Nos
				experts s'occupent de vos réseaux sociaux, du rédactionnel et des publications… vous laissant
				ainsi vous concentrer sur l'essentiel. Plus de temps, c'est aussi un super plus pour exprimer
				votre talent !
			</p>
		</div>

		<!-- Card 3 -->
		<div
			class="bg-white p-8 border-t-2 border-primary rounded-lg shadow-lg flex flex-col items-start text-left text-primary"
		>
			<div class="mb-4">
				<!-- Icon (You can replace with appropriate SVG) -->
				<div class="bg-tertiary text-white p-3 rounded-full">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="2"
						stroke="currentColor"
						class="h-8 w-8"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M12 8v4m0 4h.01M12 8v4m0 4h.01M12 8v4m0 4h.01"
						/>
					</svg>
				</div>
			</div>
			<h3 class="text-xl font-semibold mb-2 text-gray-800 playfair h-[70px]">
				Profitez d’un suivi personnalisé
			</h3>
			<p class="text-gray-400 text-sm playfair">
				Parce que vous êtes unique, nous vous accompagnons de façon unique. Ensemble, nous
				définissons votre image, vos différences, et une stratégie sur mesure. Notre équipe est à
				l'écoute, réactive et très préoccupée par votre épanouissement et votre réussite. Bien
				au-delà du succès, nous visons votre épanouissement et une longue collaboration.
			</p>
		</div>
	</div>
</section>

<!-- SECTION 3  -->
<section id="Résultats" class="bg-white py-28 px-6 lg:px-20">
	<div class="max-w-7xl mx-auto">
		<!-- Section Header -->

		<!-- Result Cards -->
		<div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
			<div class="">
				<h2 class="text-3xl font-semibold mb-4 playfair">
					<span class="text-primary">Résultats récents</span> des modèles de l'agence {agencyName} sur
					OnlyFans et MYM
				</h2>
				<p class="text-lg text-gray-700">
					Voici les résultats et revenus qu'il est possible d'atteindre en rejoignant {agencyName}
					Agency.
				</p>
				<a href="#hero" class="text-primary font-semibold mt-2 inline-block"
					>Découvrez comment obtenir ces résultats →</a
				>
			</div>
			<!-- Card 1 -->
			<div class="bg-white border rounded-lg shadow-lg p-4">
				<div class="flex justify-between items-center mb-4">
					<h3 class="font-semibold text-lg">All time</h3>
					<span class="text-primary font-semibold text-xl">$41,301.08</span>
				</div>
				<img src={girl1} alt="Chart 1" class="w-full object-cover h-[200px]" />
				<div class="mt-4 text-gray-700">
					<p>From Jun 1, 2022 to Jul 31, 2022</p>
					<p class="font-semibold">$5,194.06 in Subscriptions</p>
				</div>
			</div>

			<!-- Card 2 -->
			<div class="bg-white border rounded-lg shadow-lg p-4">
				<div class="flex justify-between items-center mb-4">
					<h3 class="font-semibold text-lg">All time</h3>
					<span class="text-primary font-semibold text-xl">$24,786.96</span>
				</div>
				<img src={girl1} alt="Chart 2" class="w-full object-cover h-[200px]" />
				<div class="mt-4 text-gray-700">
					<p>From August 2022 to August 31, 2022</p>
					<p class="font-semibold">$3,753.66 in Subscriptions</p>
				</div>
			</div>

			<!-- Card 3 -->
			<div class="bg-white border rounded-lg shadow-lg p-4">
				<div class="flex justify-between items-center mb-4">
					<h3 class="font-semibold text-lg">All time</h3>
					<span class="text-primary font-semibold text-xl">$56,368.23</span>
				</div>
				<img src={girl1} alt="Chart 3" class="w-full object-cover h-[200px]" />
				<div class="mt-4 text-gray-700">
					<p>From Jun 1, 2022 to Sep 1, 2022</p>
					<p class="font-semibold">$8,655.43 in Subscriptions</p>
				</div>
			</div>
		</div>
	</div>
</section>

<section id="Services" class="bg-white py-28 px-6 lg:px-20">
	<div class="max-w-7xl mx-auto text-center mb-12">
		<!-- Section Title -->
		<h2 class="text-3xl lg:text-4xl font-semibold mb-4 playfair">
			<span class="text-primary">Une stratégie et un accompagnement sur mesure</span>
			<br />
			pour se démarquer sur OnlyFans et MYM
		</h2>
		<div class="flex justify-center">
			<p class=" lg:text-lg text-gray-700 max-w-2xl">
				En tant qu'agence OnlyFans et MYM, {agencyName} propose un accompagnement et des prestations
				adaptés à chaque modèle. Nos managers et manageuses spécialisés.es suivent votre compte dans
				la durée et adaptent en permanence les actions pour un rendement optimal.
			</p>
		</div>
	</div>
	<div class=" flex justify-center items-center w-full">
		<!-- Services Grid -->
		<div class="grid grid-cols-1 lg:grid-cols-2 xl:grid-cols-3 gap-8 max-w-6xl">
			<!-- Card 1 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							class="h-8 w-8"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M12 2l9.53 6.69c.87.61.87 1.91 0 2.52L12 18.8 2.47 11.21a1.5 1.5 0 010-2.52L12 2z"
							/>
						</svg>
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Définition de votre image unique</h3>
				<p>
					Si vous n'avez pas encore établi un positionnement précis et une image distincte, notre
					mission sera de les définir ensemble. Une identité marquante, unique et attachante est
					essentielle pour vous différencier et attirer vos ventes. C'est votre valeur numérique, le
					fondement de votre réussite et de votre manière de publier, pour mieux cibler votre public
					ou un niche spécifique.
				</p>
			</div>

			<!-- Card 2 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							class="h-8 w-8"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M3 3h18v18H3V3z" />
						</svg>
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Gestion de comptes MYM et OnlyFans</h3>
				<p>
					Concentrez-vous sur la création, nous gérons tout le reste pour vous ! Nos managers et
					manageuses OnlyFans et MYM vous conseillent sur le type de contenu à concevoir pour
					maximiser vos résultats. Nous nous chargeons de diffuser sur vos réseaux sociaux et
					préparons vos vidéos et légendes efficaces et optimisées. Ce cycle vertueux sera le moteur
					de votre succès !
				</p>
			</div>

			<!-- Card 3 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							class="h-8 w-8"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
						</svg>
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Marketing et promotion</h3>
				<p>
					Nombre de followers, conversion en abonnés payants, revenus, tout repose au départ sur
					votre notoriété. Nous déployons les actions en ligne qui mettent en avant vos plateformes
					et créateurs, soudures, et accroissement votre flux de visiteurs. Via de multiples canaux
					de communication gratuits et payants, nous amenons de nouveaux fans à vous découvrir
					chaque jour.
				</p>
			</div>

			<!-- Card 4 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							class="h-8 w-8"
						>
							<path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
						</svg>
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Conseil, accompagnement, formation</h3>
				<p>
					Nous sommes fiers d'accompagner nos modèles dans leur chemin vers la réussite, offrant un
					service personnalisé. Notre approche bienveillante inclut des conseils sur la
					présentation, les relations et la monétisation de votre fan base. Vous êtes guidé.e vers
					le succès, bénéficiant de l'expertise de coaches dédiés à votre réussite.
				</p>
			</div>

			<!-- Card 5 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							class="h-8 w-8"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M12 8v4m0 4h.01M12 8v4m0 4h.01M12 8v4m0 4h.01"
							/>
						</svg>
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Planification et inspiration</h3>
				<p>
					Pour vous aider à surmonter d'éventuels manques d'inspiration ou de motivation, nous
					effectuons une veille constante des tendances. Nous vous apportons des idées de contenu
					inspirantes jusqu'à la date des posts. Ces idées sont alors mises en avant, avec des
					visuels et des concepts créatifs. Renforcez votre présence pour vous démarquer.
				</p>
			</div>

			<!-- Card 6 -->
			<div class="bg-secondary text-white p-6 rounded-lg shadow-lg border-t-2 border-primary">
				<div class="mb-4">
					<!-- Replace with an appropriate icon -->
					<div class="bg-primary text-white p-3 rounded-full inline-block">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="2"
							stroke="currentColor"
							class="h-8 w-8"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M12 8v4m0 4h.01M12 8v4m0 4h.01M12 8v4m0 4h.01"
							/>
						</svg>
					</div>
				</div>
				<h3 class="text-xl font-semibold mb-4 playfair">Assistance et support</h3>
				<p>
					Bénéficiez d'une assistance complète pour gérer vos comptes OnlyFans et MYM. L'agence se
					charge des problèmes techniques, de l'analyse des performances, des aspects juridiques, et
					du marketing. Nous veillons à protéger vos droits, en sécurisant vos contenus. Les
					solutions d'assistance sont mises à votre disposition pour résoudre tout problème et vous
					assurer une tranquillité d'esprit.
				</p>
			</div>
		</div>
	</div>

	<!-- Call to Action -->
	<div class="mt-12 text-center flex justify-center">
		<a href="#hero" class="linkButtonPrimary"> Rejoignez {agencyName} </a>
	</div>
</section>

<section id="A propos" class="bg-white py-28 px-6 lg:px-20">
	<div class="max-w-7xl mx-auto">
		<!-- Top Section: Image and Description -->
		<div class="lg:flex lg:items-center lg:space-x-12">
			<!-- Image -->
			<div class="flex-shrink-0 mb-8 lg:mb-0">
				<img
					src={buis}
					alt="Team"
					class="rounded-lg shadow-lg w-full lg:w-auto max-h-[500px] object-contain"
				/>
			</div>

			<!-- Description -->
			<div>
				<h2 class="text-3xl lg:text-4xl font-semibold mb-4 playfair">
					{agencyName}, <span class="text-primary">une agence OnlyFans et MYM</span> qui couvre tout
					le spectre du management de comptes
				</h2>
				<p class=" text-gray-700 mb-4">
					{agencyName}, agence française dédiée au management de comptes OnlyFans et MYM, a pour
					mission d'optimiser la visibilité des créatrices de contenu et d'accroître leurs revenus
					tout en garantissant leur bien-être et un gain de temps précieux.
				</p>
				<p class=" text-gray-700">
					Notre équipe de manageuses et managers OnlyFans et MYM propose une gamme de services
					incluant gestion de vos comptes et réseaux sociaux, élaboration d'une image de marque
					cohérente, conseil et assistance sur les aspects créatifs, juridiques et financiers. Nous
					veillons également à la protection de vos contenus et à l'action contre les partages
					illégaux.
				</p>
			</div>
		</div>

		<!-- Values Section -->
		<div class="flex justify-center items-center space-x-4 text-center my-20 playfair">
			<div class="border-b-2 border-gray-300 flex-grow"></div>
			<span class="text-xl font-semibold">Humanité</span>
			<div class="border-b-2 border-gray-300 flex-grow"></div>
			<span class="text-xl font-semibold">Confiance</span>
			<div class="border-b-2 border-gray-300 flex-grow"></div>
			<span class="text-xl font-semibold">Bienveillance</span>
			<div class="border-b-2 border-gray-300 flex-grow"></div>
			<span class="text-xl font-semibold">Respect</span>
			<div class="border-b-2 border-gray-300 flex-grow"></div>
		</div>

		<!-- Call to Action Section -->
		<div
			class="bg-secondary text-white mt-12 p-8 rounded-lg shadow-lg flex flex-col lg:flex-row lg:items-center"
		>
			<div class="lg:w-2/3">
				<h3 class="text-2xl font-semibold mb-4">Pourquoi choisir {agencyName} ?</h3>
				<p class="text-lg mb-4">
					Si nous ne deviez retenir qu'une seule raison de travailler avec nous, nous pensons que ce
					serait la suivante : {agencyName} est une agence résolument humaine. Nous traitons nos modèles
					comme telles, avec respect et bienveillance. Nous sommes attentifs à votre bien-être et épanouissement
					tout au long de notre relation. C'est notre identité profonde et notre fierté.
				</p>
				<p class="text-lg">
					Faites appel à {agencyName} et propulsez votre carrière, sans compromis.
				</p>
			</div>
			<div class="lg:w-1/3 mt-4 lg:mt-0 lg:pl-8 text-center lg:text-left">
				<a
					href="#hero"
					class="bg-primary text-black py-3 px-8 rounded-lg font-semibold hover:bg-yellow-700 inline-block mt-4 lg:mt-0"
				>
					Rejoignez {agencyName} →
				</a>
			</div>
		</div>
	</div>
</section>

<footer class="bg-primary py-8 px-6 lg:px-20 text-white">
	<div class="max-w-7xl mx-auto text-center">
		<!-- Logo -->
		<div class="mb-6">
			<img src={logo} alt={agencyName} class="mx-auto h-16 rounded-full" />
		</div>

		<!-- Agency Name -->
		<h2 class="text-2xl font-semibold mb-6">{agencyName}</h2>

		<!-- Navigation Links -->
		<nav class="mb-6">
			<ul class="flex justify-center space-x-6">
				<li><a href="#Solution" class="hover:underline">Solution</a></li>
				<li><a href="#Resultas" class="hover:underline">Résultats</a></li>
				<li><a href="#Services" class="hover:underline">Services</a></li>
				<li><a href="#A propos" class="hover:underline">À propos</a></li>
				<li><a href="#FAQ" class="hover:underline">FAQ</a></li>
				<li><a href="#Contact" class="hover:underline">Contact</a></li>
			</ul>
		</nav>

		<!-- Social Media Icons -->
		<div class="flex justify-center space-x-6 mb-6">
			<!-- Instagram Icon -->
			<a
				href="https://www.instagram.com"
				class="text-secondary hover:text-tertiary"
				aria-label="Instagram"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="h-8 w-8"
					viewBox="0 0 24 24"
				>
					<path
						d="M12 2.163c3.204 0 3.584.012 4.85.07 1.366.062 2.633.312 3.608 1.287.975.975 1.225 2.242 1.287 3.608.058 1.266.07 1.646.07 4.85s-.012 3.584-.07 4.85c-.062 1.366-.312 2.633-1.287 3.608-.975.975-2.242 1.225-3.608 1.287-1.266.058-1.646.07-4.85.07s-3.584-.012-4.85-.07c-1.366-.062-2.633-.312-3.608-1.287-.975-.975-1.225-2.242-1.287-3.608-.058-1.266-.07-1.646-.07-4.85s.012-3.584.07-4.85c.062-1.366.312-2.633 1.287-3.608.975-.975 2.242-1.225 3.608-1.287 1.266-.058 1.646-.07 4.85-.07zm0-2.163c-3.257 0-3.667.013-4.947.072-1.428.065-2.905.332-3.993 1.42-1.088 1.088-1.355 2.565-1.42 3.993-.059 1.281-.072 1.691-.072 4.947s.013 3.667.072 4.947c.065 1.428.332 2.905 1.42 3.993 1.088 1.088 2.565 1.355 3.993 1.42 1.281.059 1.691.072 4.947.072s3.667-.013 4.947-.072c1.428-.065 2.905-.332 3.993-1.42 1.088-1.088 1.355-2.565 1.42-3.993.059-1.281.072-1.691.072-4.947s-.013-3.667-.072-4.947c-.065-1.428-.332-2.905-1.42-3.993-1.088-1.088-2.565-1.355-3.993-1.42-1.281-.059-1.691-.072-4.947-.072z"
					/>
					<path
						d="M12 5.838a6.162 6.162 0 1 0 0 12.324 6.162 6.162 0 0 0 0-12.324zm0 10.162a3.999 3.999 0 1 1 0-7.998 3.999 3.999 0 0 1 0 7.998zm6.406-11.845a1.44 1.44 0 1 0 0 2.88 1.44 1.44 0 0 0 0-2.88z"
					/>
				</svg>
			</a>

			<!-- Facebook Icon -->
			<a
				href="https://www.facebook.com"
				class="text-secondary hover:text-tertiary"
				aria-label="Facebook"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="h-8 w-8"
					viewBox="0 0 24 24"
				>
					<path
						d="M22.676 0h-21.351c-.73 0-1.325.594-1.325 1.324v21.351c0 .73.594 1.325 1.325 1.325h11.492v-9.284h-3.124v-3.622h3.124v-2.671c0-3.1 1.893-4.788 4.656-4.788 1.325 0 2.462.099 2.795.142v3.241l-1.917.001c-1.504 0-1.795.716-1.795 1.764v2.311h3.587l-.467 3.622h-3.12v9.284h6.118c.73 0 1.325-.594 1.325-1.325v-21.35c0-.731-.595-1.325-1.325-1.325z"
					/>
				</svg>
			</a>

			<!-- WhatsApp Icon -->
			<a
				href="https://www.whatsapp.com"
				class="text-secondary hover:text-tertiary"
				aria-label="WhatsApp"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="h-8 w-8"
					viewBox="0 0 24 24"
				>
					<path
						d="M16.555 13.412c-.265-.131-1.574-.777-1.819-.867-.242-.086-.419-.131-.595.132-.175.262-.681.867-.837 1.045-.155.175-.307.197-.573.065-.265-.131-1.118-.41-2.131-1.307-.788-.705-1.319-1.573-1.473-1.838-.155-.262-.017-.403.116-.532.119-.119.263-.309.394-.465.132-.154.175-.263.264-.438.087-.175.044-.328-.022-.465-.065-.131-.596-1.437-.816-1.976-.215-.517-.433-.446-.596-.456-.155-.013-.328-.016-.503-.016-.175 0-.46.065-.7.328-.242.262-.918.896-.918 2.185 0 1.287.94 2.531 1.07 2.705.131.175 1.855 2.841 4.501 3.985.629.272 1.118.434 1.501.559.63.2 1.2.175 1.654.106.504-.075 1.573-.643 1.794-1.268.22-.624.22-1.159.154-1.268-.065-.109-.242-.175-.507-.309zm-4.555 8.588c-1.333 0-2.632-.347-3.779-.1c0 0-.874 1.228-2.086 1.65c0 0 .407-1.288.497-1.512c-1.178-.922-2.034-2.114-2.486-3.507c-.494-1.522-.494-3.19 0-4.712c.47-1.429 1.361-2.649 2.486-3.506c.954-.769 2.062-1.269 3.227-1.48c1.174-.211 2.395-.061 3.479.44c1.084.5 2.035 1.267 2.798 2.235c.76.967 1.288 2.149 1.52 3.379c.23 1.23.132 2.49-.302 3.668c-.365 1.034-1.084 1.967-1.98 2.587c-.896.62-1.998.943-3.132.94z"
					/>
				</svg>
			</a>
		</div>

		<!-- Copyright Text -->
		<p class="text-sm mb-4">Copyright © 2024 • {agencyName}. Tous droits réservés.</p>

		<!-- Legal Links -->
		<div class="flex justify-center space-x-4 text-sm">
			<a href="#hero" class="hover:underline">Mentions légales</a>
			<span class="text-gray-400">|</span>
			<a href="#hero" class="hover:underline">Politique de confidentialité</a>
			<span class="text-gray-400">|</span>
			<a href="#hero" class="hover:underline">Politique de cookies</a>
		</div>
	</div>

	<!-- Bottom Bar -->
	<div class="bg-primary-dark py-2 mt-8 text-center text-sm">
		<p class="text-gray-800">
			Design, textes et dev par <a href="#hero" class="text-white hover:underline">PB</a>
		</p>
	</div>
</footer>
