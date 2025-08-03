<script>
	import '../app.css';
	import Navbar from '$lib/components/Navbar.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
	<title>Burbsec | The World's Most Fun InfoSec Meetup Events!</title>
	<meta name="description" content="Join Burbsec, the world's most fun information security meetup network! Connect with cybersecurity professionals, ethical hackers, and infosec enthusiasts across Chicago, Las Vegas, Galway and more. A welcoming community for those seeking Chicago hacker meetups and security networking events." />
	
	<!-- Open Graph Tags -->
	<meta property="og:title" content="Burbsec | The World's Most Fun InfoSec Meetup Events!" />
	<meta property="og:description" content="Join Burbsec, the world's most fun information security meetup network! Connect with cybersecurity professionals, ethical hackers, and infosec enthusiasts across Chicago, Las Vegas, Galway and more." />
	
	<!-- Twitter Card Tags -->
	<meta name="twitter:title" content="Burbsec | The World's Most Fun InfoSec Meetup Events!" />
	<meta name="twitter:description" content="Join Burbsec, the world's most fun information security meetup network! Connect with cybersecurity professionals, ethical hackers, and infosec enthusiasts." />
	
	<!-- Structured Data (JSON-LD) -->
	{@html `<script type="application/ld+json">
	{
		"@context": "https://schema.org",
		"@type": "Organization",
		"name": "Burbsec Network",
		"alternateName": "Burbsec",
		"description": "The world's most fun information security meetup network connecting cybersecurity professionals, ethical hackers, and infosec enthusiasts.",
		"url": "https://burbsec.github.io/",
		"logo": "https://burbsec.github.io/images/hacker_shield.png",
		"image": "https://burbsec.github.io/images/hacker_shield.png",
		"foundingDate": "2020",
		"sameAs": [
			"https://www.meetup.com/burbsec/",
			"https://discord.gg/burbsec"
		],
		"contactPoint": {
			"@type": "ContactPoint",
			"contactType": "Community Support",
			"url": "https://tinyurl.com/burbchat"
		},
		"areaServed": [
			{
				"@type": "City",
				"name": "Chicago",
				"addressRegion": "IL",
				"addressCountry": "US"
			},
			{
				"@type": "City",
				"name": "Las Vegas",
				"addressRegion": "NV",
				"addressCountry": "US"
			},
			{
				"@type": "City",
				"name": "Galway",
				"addressCountry": "IE"
			}
		],
		"event": [
			{
				"@type": "Event",
				"name": "Burbsec Chicago Meetup",
				"description": "Monthly information security meetup in Chicago",
				"eventSchedule": {
					"@type": "Schedule",
					"repeatFrequency": "P1M",
					"byDay": "Thursday"
				},
				"location": {
					"@type": "Place",
					"name": "Chicago",
					"address": {
						"@type": "PostalAddress",
						"addressLocality": "Chicago",
						"addressRegion": "IL",
						"addressCountry": "US"
					}
				},
				"organizer": {
					"@type": "Organization",
					"name": "Burbsec Network"
				}
			}
		],
		"keywords": "information security, cybersecurity, hacking, infosec, meetup, chicago, security professionals, ethical hacking, penetration testing, cybersecurity community, security events, networking, CISSP, CEH, security training, vulnerability assessment, incident response, malware analysis, digital forensics, security awareness, chicago hacker meetup, chicago security community, defcon chicago, chicago infosec community"
	}
	</script>`}
</svelte:head>

<Navbar />
<main>
	<slot />
</main>
<Footer />

<style>
	:global(body) {
		background-color: #15202b;
		min-height: 100vh;
		color: white;
	}
	
	main {
		min-height: calc(100vh - 200px);
	}
</style>