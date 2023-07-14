<script lang="ts">
  type AppView = "start" | "charge"
  let appView: AppView = "start"

  function setView(view: AppView) {
    appView = view
  }

</script>
<div class="container">
{#if appView === 'start'}
<h2> Arc </h2>
<div> Logo Goes here </div>
{/if}
<div class="button-container">
<button class="menu-button" on:click={() => setView('start')}>
Start
</button>
<button class="menu-button" on:click={() => setView('charge')}>
Charge View
</button>
</div>
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }
  .button-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
  .menu-button {
    width: 200px;
  }
</style>
