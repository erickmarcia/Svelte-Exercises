<script>
  import Datos from './Datos.svelte';

  export let name;

  let nombreCompleto = {
    nombre: 'Erick',
    apellidos: 'Marcia',
  };
</script>


<h1>Hola {name}!</h1>
<Datos {...nombreCompleto} />