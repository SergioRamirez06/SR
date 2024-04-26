<script>
  import ParImpar from "./par-impar.svelte";
  let valor = 0;
  const listenInput = (event) => (valor = event.target.value);
</script>

<main>
  <!-- <ParImpar ParImpar={6} />

  <ParImpar ParImpar={20} />

  <ParImpar ParImpar={0} /> -->

  <ParImpar ParImpar={valor} />

  <input
    type="text"
    class="form form-control"
    value={valor}
    on:input={listenInput}
  />
</main>
