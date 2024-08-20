<script>
	import '../app.css';
	import logo from '$lib/images/logo.png';
	import girl from '$lib/images/girl1.png';
	import buis from '$lib/images/buiss3.png';
	import concu from '$lib/images/concu.png';
	import marketing from '$lib/images/marketing.png';
	import motivation from '$lib/images/motivation.png';
	import argent from '$lib/images/argent2.png';
	import timeplus from '$lib/images/timeplus.png';
	import perso from '$lib/images/perso.png';
	import unique from '$lib/images/unique.png';
	import gestion from '$lib/images/gestion.png';
	import vente from '$lib/images/vente.png';
	import formation from '$lib/images/formation.png';
	import planification from '$lib/images/planification.png';
	import assistance from '$lib/images/assistance.png';
	import result1 from '$lib/images/result1.png';
	import result2 from '$lib/images/result3.png';
	import Navbar from '../components/Navbar.svelte';
	import Section1 from '../components/Section1.svelte';
	import Hero from '../components/Hero.svelte';
	import Solutions from '../components/Solutions.svelte';
	import Resultats from '../components/Resultats.svelte';
	import Services from '../components/Services.svelte';
	import About from '../components/About.svelte';
	import Footer from '../components/Footer.svelte';
	import Faq from '../components/FAQ.svelte';
	import Contact from '../components/Contact.svelte';
	import { Toaster } from 'svelte-sonner';

	const agencyName = 'Mia Prestige';
	const email = 'mia.agencypro@gmail.com';
</script>

<svelte:head>
	<title>{agencyName}</title>
	<meta name="description" content={agencyName} />
</svelte:head>

<Toaster richColors />

<Navbar />

<Hero {agencyName} />

<Section1 {concu} {marketing} {motivation} {girl} />

<Solutions {agencyName} {argent} {timeplus} {perso} />

<Resultats {agencyName} {result1} {result2} />

<Services {agencyName} {unique} {gestion} {vente} {formation} {planification} {assistance} />

<About {agencyName} {buis} />

<Contact {agencyName} />

<Faq {agencyName} {email} />

<Footer {agencyName} {logo} />
