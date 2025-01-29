<script>
  let num1 = 0
  let num2 = 0
  let resultado = undefined


  function sumar(){
    resultado = num1 + num2
  }

  function restar(){
    resultado = num1 - num2
  }

  function multi(){
    resultado = num1 * num2
  }

  function divi(){
    resultado = num1 / num2
  }
</script>

<main>
  <h1>Escribe un numero en cada casilla</h1>
  <input type="number" bind:value={num1}>
  <input type="number" bind:value={num2}>

  <br>

  <button on:click={sumar}>
    +
  </button>

  <button on:click={restar}>
    -
  </button>

  <button on:click={multi}>
    *
  </button>

  <button on:click={divi}>
    %
  </button>

  <br>
    <h3>Resultado</h3>
    {resultado}
</main>


<style>
  main{
    background-color: pink;
  }

</style>
