<script>
    import Button from "../../components/Button.svelte";
    import Todo from "./Todo.svelte";

    let count = 0


    const addTodo = () => count += 1
    const clicked = () => console.log('clicked')
</script>



<h1>Todo App</h1>


<form>
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

<ul id="todo_list">
    <li>
        <Todo />
    </li>
    <li>
        <Todo />
    </li>
    <li>
        <Todo />
    </li>
</ul>

<Todo on:click={clicked}/>
<Todo on:click={clicked}/>
<Todo on:click={clicked}/>

<div>
    <p>{`there are ${count} pending tasks`}</p>
</div>



<style>
    input {
        font-size: inherit;
    }
</style>