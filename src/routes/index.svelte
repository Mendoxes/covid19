<script context="module">
	export const prerender = true;
	import CovidStats from "../components/CovidStat.svelte"
	import CovidChart from "../components/CovidChart.svelte"
	import TableContainer from "../components/TableContainer.svelte"
</script>



<svelte:head>
	<title>Home</title>

</svelte:head>

<CovidStats />
<CovidChart />
<TableContainer />

<section>

</section>


