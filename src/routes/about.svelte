<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>About Covid19</title>
</svelte:head>
<div class="section header">
<div class="container">
<h1>About</h1>
<p>The data used in this app came from <a href="https://covidtracking.com/data/api">Covid Tracking</a> if you want to learn more visit their site</p>

</div>
</div>
<style>
	p{
		padding:2rem 1rem;
	}
	/* .content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	} */
</style>
