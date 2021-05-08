<script context="module" lang="ts">
    export async function load({ page }) {
      return {
        props: {
          state: page.params.state
        },
      };
    }
  </script>
  
  <script>
    	import CovidStats from "../components/CovidStat.svelte"
	import CovidChart from "../components/CovidChart.svelte"
	import TableContainer from "../components/TableContainer.svelte"
    export let state;
  </script>
  
  params: {state} <br />

  <CovidStats />
<CovidChart />




<!-- <script context ="module">

export async function load(page){
return {state: page.params.["state"] };

}
</script>

<script>export let state;


</script>
<h1>{state}</h1> -->