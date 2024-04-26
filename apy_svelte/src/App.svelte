<script>
  export const apy = async () => {
    const url = await "https://pokeapi.co/api/v2/pokemon/ditto";
    const resp = await fetch(url);
    const { abilities, name } = await resp.json();
    console.log({ abilities, name });
  };
  const poke = apy();
</script>

<h1>{JSON.stringify(poke)}</h1>
