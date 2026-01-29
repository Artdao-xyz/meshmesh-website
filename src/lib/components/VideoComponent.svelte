<script lang="ts">
	import VideoPlayButton from './VideoPlayButton.svelte';
	import VideoModal from './VideoModal.svelte';
	
	let isModalOpen = false;
	
	function handlePlayClick() {    
		// isModalOpen = true;
		console.log('Play button clicked');
	}
	
	function handleCloseModal() {   
		// isModalOpen = false;
		console.log('Close modal clicked');
	}
</script>

<VideoPlayButton onClick={handlePlayClick} />
<VideoModal isOpen={isModalOpen} onClose={handleCloseModal} />
