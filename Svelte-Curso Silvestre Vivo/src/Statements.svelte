<script>

  //  Dentro de las sintaxis de reactividad tenemos

  // imprimir en consola
  $: console.log(variable);

  // expresiones de js
  $: {
    //expresion
  }

  // poner condicionales
  $: if (argumento) {
    // variable que retornamos
  } else {
    // variable que retornamos
  }

  // loop
  $: for (let index = 0; index < array.length; index++) {
    const element = array[index];
  }

  // funciones definidas como variables
  $; variable = argumento => {
    //return
  };

  // funciones asycronicas
  $: async () => {
    bar = await Promise.resolve(argumento);
  };

  // variables propiedades de un objeto
  // para que este funciones debemos de ponerlo todo dentro de parentesis
  $: ({ a, b } = objeto);


</script>