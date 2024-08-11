<script>
	let numbers = [1, 2, 3, 4];

	function addNumber() {
		numbers = [...numbers, numbers.length + 1]; // copy the previous elemet and add next one in array
	}

	$: sum = numbers.reduce((total, currentNumber) => total + currentNumber, 0);
</script>

<p>{numbers.join(' + ')} = {sum}</p>

<button on:click={addNumber}>
	Add a number
</button>
