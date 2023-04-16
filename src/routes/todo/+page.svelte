<script>
    import Button from "../../components/Button.svelte";

    let count = 0
    const addTodo= () => count += 1
</script>



<h1>Todo App</h1>

<form >
    <input type="text" placeholder="add todo">
    <button on:click={addTodo} type="submit">+</button>
</form>

<div class="todo">
    <span>sample todo</span>
    <Button>del</Button>
</div>

<div>
    <p>{`there are ${count} pending tasks`}</p>
</div>



<style>
    .todo {
        background-color: lightgray;
    }
</style>