<script>

  // import style from '../src/utils/styles';

  //  console.log('%c Primitivas');

  // let a = 'inmutable';

  // a.toLocaleUpperCase();

  // console.log('a', a);

  // let b = a.toLocaleUpperCase();

  // console.log('b', b);

  // trabajando con array 

  // console.log('% c Objetos y Arrays', style);

  let c = [1, 2, 3, 4];

  c.push(5);

  console.log('c', c);

  // Trabajando con objetos

  let d = {
    propi: 'uno',
  };

  d.prop2 = 'dos';

  console.log('d', d)


  // Metodos o Sintaxis que permiten operar de forma inmutable para operar con array u objetos

  console.log('% Objectos/Arrays inmutables');

  let e = [1, 2, 3, 4];

  // ...e (Srpint Operator)
  let f = [...e, 5];

  console.log('e', e);
  console.log('f', f);


  // Metodos asociados a inmutabilidad

  console.log('% Metodos inmutables Arrays/Objetos');

  let g = [1, 2, 3, 4];

  let h = [5, 6, 7, 8];


  // unimos los 2 arrays
  console.log([...g, ...h]);

  // concatenacion
  console.log(g.concat(h));

  //Obtener todos aquellos elementos menores a 2
  console.log(g.filter(i => i < 2));

  // Imprimir un nuevo arrays basado en mi array inicial y a;adirle 10 unidades
  console.log(g.map(i => i + 10));

  // si imprimimos nuestro valor inicial de los que partiamos ej> g, este aun mantiene esos valores
  console.log('g', g);

</script>