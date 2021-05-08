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
  
  <!-- params: {state} <br /> -->

  <svelte:head>
    <title>Covid 19</title>
  
  </svelte:head>
  <div class="section header">
  
  <div class="container">
  
    <h1>Covid 19 - {state}</h1>
  
  </div></div>
  

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