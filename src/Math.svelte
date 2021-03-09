<script>
    let num1;
    let num2;
    $: result = num1  * num2;
</script>

<h2>Math!</h2>
<input bind:value={num1}> x <input bind:value={num2}> = {result}