<script>
  let tableData = [
    {
      id: 1,
      amount: "$100.00",
      date: "2020-01-01",
      description: "Payment for January",
      category: "Payment",
      type: "Income",
    },
    {
      id: 2,
      amount: "$200.00",
      date: "2020-01-01",
      description: "Payment for January",
      category: "Payment",
      type: "Income",
    },
    {
      id: 3,
      amount: "$300.00",
      date: "2020-01-01",
      description: "Payment for January",
      category: "Payment",
      type: "Income",
    },
  ];
</script>

<div class="transactions-table">
  <table>
    <tr class="header-row">
      <!-- table header row -->
      <td>Id</td>
      <td>Date</td>
      <td>Amount</td>
      <td>Description</td>
      <td>Category</td>
      <td>Type</td>
    </tr>
    {#each tableData as transaction}
      <tr class="transaction-row">
        <td>{transaction.id}</td>
        <td>{transaction.date}</td>
        <td>{transaction.amount}</td>
        <td>{transaction.description}</td>
        <td>{transaction.category}</td>
        <td>{transaction.type}</td>
      </tr>
    {/each}
  </table>
</div>

<style>
  .header-row {
    background-color: #f5f5f5;
  }
</style>
