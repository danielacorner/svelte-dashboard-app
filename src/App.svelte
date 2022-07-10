<script>
  import Dashboard from "./lib/Dashboard/Dashboard.svelte";
  import LeftNavPanel from "./lib/LeftNavPanel/LeftNavPanel.svelte";
</script>

<main>
  <div class="left-column">
    <LeftNavPanel />
  </div>
  <div class="right-column">
    <Dashboard />
  </div>
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  }

  main {
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
</style>
