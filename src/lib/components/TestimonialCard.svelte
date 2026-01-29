<script lang="ts">
	export let quote: string;
	export let name: string;
	export let title: string;
</script>

<div class="bg-linear-to-b from-border-white to-[#929292] rounded-form p-[3px] w-[280px] shrink-0 shadow-(--shadow-card) md:w-[430px] md:max-w-[430px]">
	<div class="bg-card-gray rounded-form px-6 py-8 md:p-9 h-[250px] flex flex-col gap-form-container-gap">
		<div class="flex-1 flex flex-col items-center w-full">
			<p class="font-normal text-lg md:text-2xl leading-[1.4] text-text-primary text-center m-0 whitespace-pre-wrap w-full">
				{quote}
			</p>
		</div>
		<div class="flex justify-between items-start w-full font-geist-mono font-medium md:text-lg leading-[1.2] tracking-[-1px] text-center whitespace-nowrap">
			<span class="text-text-primary">{name}</span>
			<span class="text-text-secondary">{title}</span>
		</div>
	</div>
</div>
