<script>

  import Triple from './Triple.svelte';
  let numero = 0;

  function handleclick() {
    numero += 1;
  }

  $: numeroDoble = numero * 2;
</script>

<button on:click={handleclick}>{numero}</button>

<!-- /*Reactividad es hacer que una variable reaccione en función del cambio de otra variable */ -->
<!-- <button on:click={()=> (numero += 1)}>{numero}</button> -->


<p>{numeroDoble} es el doble de {numero}</p>


<Triple {numero} />