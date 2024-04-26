<script>
  export let ParImpar;
  let resultado;
  $: if (ParImpar === 0) resultado = "neutro";
  else if (ParImpar % 2 === 0) resultado = "par";
  else resultado = "impar";
</script>

<p>el numero {ParImpar} es {resultado}</p>

<style>
  p {
    color: rgb(34, 5, 112);
    font-family: Arial, Helvetica, sans-serif;
    font-size: 25px;
  }
</style>
