<script>
  import Router from 'svelte-spa-router';
  import Navigation from './components/Navigation/Navigation.svelte';
  import { routes } from './routes/index.js';
</script>

<Navigation />
<main>
  <Router {routes} />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
   	width: 80%;
    margin: 0 auto;
  }
</style>
