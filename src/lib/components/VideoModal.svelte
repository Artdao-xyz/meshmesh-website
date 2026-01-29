<script lang="ts">
	export let isOpen: boolean = false;
	export let onClose: () => void;
</script>

<!-- Create your video html here -->
{#if isOpen}
	<!-- Modal backdrop -->
	<div
		class="fixed inset-0 bg-black bg-opacity-75 z-50 flex items-center justify-center"
		role="dialog"
		aria-modal="true"
		aria-label="Video modal"
	>
		<!-- Modal content -->
		<div class="relative w-full max-w-4xl mx-4">
			<!-- Close button -->
			<button
				class="absolute -top-10 right-0 text-white text-2xl font-bold hover:opacity-75"
				aria-label="Close modal"
			>
				×
			</button>
		</div>
	</div>
{/if}
