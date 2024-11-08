<script>
	function onKeyDown(e) {
		switch (e.keyCode) {
			case 13:
				alert(document.querySelector('#url').value);
				break;
		}
	}
</script>

<main
	class="bg flex h-screen w-screen flex-col items-center justify-center bg-[url('background.webp')] bg-cover bg-center"
>
	<input
		type="text"
		id="url"
		on:keydown={onKeyDown}
		class="w-[40vw] rounded-full bg-gray-400 bg-opacity-40 bg-[url('return.svg')] bg-scroll bg-clip-padding bg-no-repeat px-6 py-4 text-lg text-white backdrop-blur-sm max-sm:w-[80vw]"
	/>
</main>

<style>
	textarea:focus,
	input:focus {
		outline: none;
	}

	input {
		background-position: right 20px center;
	}
</style>
