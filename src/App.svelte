<script>
  import logo from "./assets/svelte.png";
  import Dashboard from "./lib/Dashboard.svelte";
  import LeftNavPanel from "./lib/LeftNavPanel/LeftNavPanel.svelte";
</script>

<main>
  <div class="left-column">
    <LeftNavPanel />
  </div>
  <div class="right-column">
    <img src={logo} alt="Svelte Logo" />
    <h1>Hello world!</h1>
    <p>
      Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte
      apps.
    </p>

    <p>
      Check out <a href="https://github.com/sveltejs/kit#readme">SvelteKit</a> for
      the officially supported framework, also powered by Vite!
    </p>
    <Dashboard />
  </div>
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  }

  main {
    text-align: center;
    margin: 0 auto;
    display: flex;
    min-height: 100vh;
  }
  .left-column {
    height: 100%;
    min-height: 100vh;
    width: 256px;
  }
  .right-column {
    flex-grow: 1;
  }

  img {
    height: 16rem;
    width: 16rem;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4rem;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  p {
    max-width: 14rem;
    margin: 1rem auto;
    line-height: 1.35;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
