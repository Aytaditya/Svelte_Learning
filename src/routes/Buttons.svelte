<script>
    let count=0;
    $: doubled=count*2;

    function increase(){
        count=count+1;
    }


    $: if (count >= 10) {
		alert('count is dangerously high!');
        console.log('count is dangerously high!');
		//count = 0;
	}

    import Arrays from './Arrays.svelte';
</script>

<!-- svelte-ignore a11y-img-redundant-alt -->
<img src="/favicon.png" alt="Image">

<button on:click={increase}>hiiii {count} {count===1 ? "time" :"times"}</button>
<p class="gap">{count}'s double is {doubled}</p>


<Arrays/>


<style>
    button{
        border-radius: 10px;
        color: goldenrod;
        margin-top: 20px;
        font-family: 'Comic Sans MS', cursive;
        font-size: 2em;
    }
    .gap{
        margin-top: 20px;
        margin-left: 10px;
        font-size: 2em;
    }
</style>