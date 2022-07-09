<script>
  // svelte-material-icons docs: https://www.npmjs.com/package/svelte-material-icons
  import Check from "svelte-material-icons/Check.svelte";
  import ViewDashboard from "svelte-material-icons/ViewDashboard.svelte";
  import Cash from "svelte-material-icons/Cash.svelte";
  import Account from "svelte-material-icons/Account.svelte";
  import Cog from "svelte-material-icons/Cog.svelte";
  import LeftNavPanelItem from "./LeftNavPanelItem.svelte";

  let width = "24px";
  let height = "24px";
</script>

<div class="left-nav-panel">
  <div class="top">
    <LeftNavPanelItem title={"Dashboard"}>
      <ViewDashboard {width} {height} slot="icon" />
    </LeftNavPanelItem>
    <LeftNavPanelItem title={"Transactions"}>
      <Cash {width} {height} slot="icon" />
    </LeftNavPanelItem>
    <LeftNavPanelItem title={"Something"}>
      <Check {width} {height} slot="icon" />
    </LeftNavPanelItem>
  </div>

  <div class="divider" />
  <div class="bottom">
    <LeftNavPanelItem title={"Account"}>
      <Account {width} {height} slot="icon" />
    </LeftNavPanelItem>
    <LeftNavPanelItem title={"Settings"}>
      <Cog {width} {height} slot="icon" />
    </LeftNavPanelItem>
  </div>
</div>

<style>
  .left-nav-panel {
    height: 100%;
    min-height: 100vh;
    width: 100%;
    box-shadow: 1px 1px 9px 2px #0000001c;
    background: rgb(252, 251, 241);
  }
</style>
