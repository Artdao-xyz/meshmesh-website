<script lang="ts">
	function handleClick() {
		// Play button logic will go here
		console.log('Play button clicked');
	}
</script>

<button
	onclick={handleClick}
	aria-label="Play video"
	class="relative w-[100px] h-[100px] bg-transparent border-0 cursor-pointer p-0 flex items-center justify-center hover:opacity-90 transition-opacity"
>
	<div class="absolute inset-[-2.53%]">
		<img
			src="/icon-play-button.svg"
			alt="Play video"
			class="block max-w-none w-full h-full"
		/>
	</div>
</button>
