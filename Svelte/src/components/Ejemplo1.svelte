<script>
    let counter = 2;
    let isEvenMessage;
    $: isEvenMessage = counter % 2 === 0 ? 'Es par' : 'Es impar'
   
    const handleClick = () => counter++
    </script>
   <div>
        <button on:click={handleClick}>Incrementar</button>
        <span>{counter}</span>
        <span>{isEvenMessage}</span>
   </div>

  