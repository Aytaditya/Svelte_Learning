<script>
    export let name;
</script>

<div class="flex">
<p>my name is {name}</p>
<h2>Props appended above</h2>
</div>


<style>
    p,h2{
        padding: 20px;
        font-size: 2em;
        background-color: antiquewhite;
    }
    .flex{
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>