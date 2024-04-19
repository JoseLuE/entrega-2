<script>
    let count = 0;
  
    $: doubled = count * 2;
  
    function increment() {
      count += 1;
    }
  </script>
  <div>
    <h1>Numero: {count}</h1>
    <h2>Doble: {doubled}</h2>
  
    <button on:click={increment}>Increment</button>
  </div>
  
  