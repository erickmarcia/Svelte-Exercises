<script>
  // import Datos from './Datos.svelte';
  import Buttom from './Buttom.svelte';

  export let name = "emarcia";

  let disable = true;

  // let nombreCompleto = {
  //   nombre: 'Erick',
  //   apellidos: 'Marcia',
  // };

  let objeto = {
    disabled: true,
    text: 'click',
  };

  console.log('objeto', objeto);
</script>


<h1>Hola {name}!</h1>
<!-- <Datos {...nombreCompleto} /> -->

<!-- /*Esto es un componente*/ -->
<!-- <Buttom /> -->

<!-- /*Esto es un action HTML*/ -->
<!-- <button disabled>Click</button> -->

<!-- Darle valor con Javascripts -->
<!-- <button {disable}>Click</button>
<input type="text">
<a href="http://github.com/{name}">{name}</a>
<a href={`http://github.com/${name}`}>{name}</a> -->
<!-- /*Esto es un componente*/ -->
<!-- <Buttom /> -->
<Buttom {...objeto} />
{console.log('objeto', objeto)}
{@debug objeto}
<div>
  <Buttom {...objeto} />
</div>

<style>
  div :global(button) {
    border: 1px solid red;
  }
</style>