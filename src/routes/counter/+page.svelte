<script>
    import Button from '../../components/Button.svelte'
    let count  = 0;

    const increment = () => count += 1;
    const decrement = () => count -= 1;
</script>

<p>{count}</p>
<Button on:click={increment}>+</Button>
<Button on:click={decrement}>-</Button>