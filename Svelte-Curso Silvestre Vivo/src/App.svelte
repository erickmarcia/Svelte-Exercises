<script>

  import Inmutable from './Inmutable.svelte';

  let numero = [1, 2, 3, 4];

  function addNumber() {
    numero = [...numero, numero.length + 1];
  }

  // Variable reactiva
  $: suma = numero.reduce((a, b) => a + b, 0)
</script>

<p>{numero.join(' + ')}={suma}</p>

<button on:click={addNumber}>Añadir Número</button>
<Inmutable />