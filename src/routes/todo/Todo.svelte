<script>
    import Button from "../../components/Button.svelte";
</script>

<div class="todo">
    <span>sample todo</span>
    <Button on:click>del</Button>
</div>

<style>
     .todo {
        background-color: lightgray;
    }
</style>