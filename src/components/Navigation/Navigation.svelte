<script>
  import { link } from 'svelte-spa-router';
  import { routesNav } from '../../constants/index.js';
</script>

<div>
  <nav>
    <ul class="nav">
      {#each routesNav as route}
        <li key={route.name} class="nav__item">
          <a class="nav__item--link" href={route.path} use:link>
            {route.name}
          </a>
        </li>
      {/each}
    </ul>
  </nav>
</div>

<style>
  ul {
    padding: 0;
    margin: 0;
    list-style-type: none;
  }

  a {
    text-decoration: none;
  }

  .nav {
    display: flex;
    justify-content: space-between;
    height: 5vh;
  }

  .nav__item {
    width: 100%;
    height: 100%;
    padding: 0;
    margin: 0 auto;
    text-align: center;
    background-color: orangered;
    border: 1px solid white;
  }

  .nav__item--link {
    display: block;
    width: 100%;
    height: 100%;
    line-height: 5vh;
    color: white;
  }
</style>
