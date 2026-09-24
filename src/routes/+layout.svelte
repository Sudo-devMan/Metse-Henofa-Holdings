<script>
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Metse Henofa Holdings | Construction, Security & Business Solutions in Johannesburg</title>
</svelte:head>
{@render children()}
