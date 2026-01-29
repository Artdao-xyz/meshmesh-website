<script lang="ts">
	export let quote: string;
	export let name: string;
	export let title: string;
</script>

<div class="bg-card-gray border-[3px] border-border-white rounded-form px-10 py-9 w-full max-w-[430px] h-[250px] flex flex-col gap-form-container-gap shadow-[var(--shadow-card)] md:w-[430px]">
	<div class="flex-1 flex flex-col items-center w-full">
		<p class="font-sans font-normal text-2xl leading-[1.4] text-text-primary text-center m-0 whitespace-pre-wrap w-full">
			{quote}
		</p>
	</div>
	<div class="flex justify-between items-start w-full font-mono font-medium text-lg leading-[1.2] tracking-[-1px] text-center whitespace-nowrap">
		<span class="text-text-primary">{name}</span>
		<span class="text-text-secondary">{title}</span>
	</div>
</div>
