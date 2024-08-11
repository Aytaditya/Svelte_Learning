<script>
	import Nested from './Nested.svelte';
    import './app.css';
    import Buttons from './Buttons.svelte';

    let string = `this string contains some <strong>HTML!!!</strong>`;
    // this string will be used as strong html content if @html is used if not it will show as plain text ending with </strong>
</script>

<p>This is a paragraph.</p>
<Nested />
<p>{@html string}</p>
<p class="bg">{string}</p>

<Buttons/>



<style>
	p {
		color: goldenrod;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
    .bg{
        background-color: rgb(237, 169, 169);
    }

</style>
