<script>
    let count = 0
    const yup = () => count += 1
</script>




<h1>Todo App</h1>

<form >
    <input type="text" placeholder="add todo">
    <button on:click={yup} type="submit">+</button>
</form>

<div class="todo">
    <span>sample todo</span>
    <button>del</button>
</div>

<div>
    <p>{`there are ${count} pending tasks`}</p>
</div>



<style>
    .todo {
        background-color: lightgray;
    }
</style>