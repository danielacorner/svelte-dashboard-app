<script>
  import TransactionsTable from "./TransactionsTable.svelte";
</script>

<div class="dashboard-items">
  <div class="item">
    <h1 class="title">Dashboard</h1>
    <p class="subtitle">
      Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte
      apps.
    </p>
  </div>
  <div class="item">
    <h2 class="title">Transactions</h2>
    <TransactionsTable />
  </div>
</div>

<style>
  .dashboard-items {
    padding-left: 2em;
    display: flex;
    flex-direction: column;
    gap: 1em;
  }
</style>
