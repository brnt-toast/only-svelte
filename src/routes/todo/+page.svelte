<script>
    import Button from "../../components/Button.svelte";

    let count = 0
    const addTodo= () => count += 1
</script>



<h1>Todo App</h1>

<form >
    <input 
        id="todo_input" 
        name='todo_input' 
        type="text" 
        placeholder="add todo">
    <Button 
        on:click={addTodo} 
        type="submit">
        +
    </Button>
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
    input {
        font-size: inherit;
    }
    
</style>