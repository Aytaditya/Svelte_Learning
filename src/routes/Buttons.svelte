<script>
    let count=0;
    function increase(){
        count=count+1;
    }
</script>


<button on:click={increase}>hiiii {count} {count===1 ? "time" :"times"}</button>

<style>
    button{
        border-radius: 10px;
        color: goldenrod;
        margin-top: 20px;
        font-family: 'Comic Sans MS', cursive;
        font-size: 2em;
    }
</style>