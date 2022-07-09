<script>
  export let title;
</script>

<div class="left-nav-panel-item">
  <div class="left">
    <slot name="icon" />
  </div>
  <div class="right">
    <h2 class="title">{title}</h2>
  </div>
</div>

<style>
  .left-nav-panel-item {
    height: 48px;
    width: 100%;
    display: flex;
    padding: 8px 16px;
  }
  .title {
    font-size: 18px;
    font-weight: 500;
    color: #212121;
    margin-left: 16px;
  }
  .left {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 48px;
    height: 48px;
  }
  .right {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: flex-start;
    align-items: center;
  }
</style>
