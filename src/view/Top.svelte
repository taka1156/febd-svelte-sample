<script>
  let name = 'world';
</script>

<div>
  <h1>Svelte App</h1>
  <img src="./static/svelte.svg" alt="svelte logo" class="logo">
  <p class="welcome">Hello {name}!</p>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
</div>

<style>
  .welcome {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 10;
    margin: 10px;
  }

  .logo {
    height: 50%;
    width: 50%;
  }
</style>
