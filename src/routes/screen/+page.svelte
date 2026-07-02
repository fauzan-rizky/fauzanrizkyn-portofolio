<script>
  // 1. Inisialisasi state awal dengan $state()
  let innerWidth = $state(0);
  let innerHeight = $state(0);

  // 2. Gunakan $derived() sebagai pengganti $:
  let ratio = $derived(innerWidth / innerHeight);
  let isUltrawide = $derived(ratio >= 2.3);
  let isSixteenNine = $derived(ratio >= 1.7 && ratio < 1.8);
</script>

<svelte:window bind:innerWidth bind:innerHeight />

<div>
  <p>Rasio Desimal: {ratio.toFixed(2)}</p>
  
  {#if isUltrawide}
    <p class="status ultrawide">🖥️ Layar kamu Ultra-Wide!</p>
  {:else if isSixteenNine}
    <p class="status normal">📺 Layar kamu Standar 16:9.</p>
  {:else}
    <p class="status">📱 Layar kamu rasio lain (atau portrait).</p>
  {/if}
</div>

<style>
  .status { font-weight: bold; }
  .ultrawide { color: purple; }
  .normal { color: green; }
</style>