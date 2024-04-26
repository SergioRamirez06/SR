<script>
  export const apy = async () => {
    const url = await "https://pokeapi.co/api/v2/pokemon";
    const resp = await fetch(url);
    const { data } = await resp.json();
    console.log(data);
  };
</script>
