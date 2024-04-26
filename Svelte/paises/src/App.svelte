<script>
  import Paises from "./lib/paises.svelte";

  const lista = [
    "colombia",
    "venezuela",
    "ecuador",
    "peru",
    "brasil",
    "argentina",
  ];
</script>

<div>
  {#each lista as pais}
    <div>
      <Paises {pais} />
    </div>
  {:else}
    no existe elementos
  {/each}
</div>

<svelte:head>
  <title>Paises De Sudamerica</title>
</svelte:head>
