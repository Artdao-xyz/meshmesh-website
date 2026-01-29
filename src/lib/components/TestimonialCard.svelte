<script lang="ts">
	export let quote: string;
	export let name: string;
	export let title: string;
</script>

<div class="bg-linear-to-b from-border-white to-[#929292] rounded-form p-[3px] w-[280px] shrink-0 shadow-(--shadow-card) md:w-[430px] md:max-w-[430px]">
	<div class="bg-card-gray rounded-form px-[40px] py-[50px] md:px-10 md:py-9 flex flex-col gap-[30px] md:gap-form-container-gap md:h-[250px]">
		<div class="flex-1 flex flex-col items-center w-full">
			<p class="font-normal text-[18px] md:text-2xl leading-[1.4] text-text-primary text-center m-0 whitespace-pre-wrap w-full">
				{quote}
			</p>
		</div>
		<div class="flex justify-between items-start w-full font-geist-mono font-medium text-[16px] md:text-lg leading-[1.2] tracking-[-0.16px] md:tracking-[-1px] text-center whitespace-nowrap">
			<span class="text-text-primary">{name}</span>
			<span class="text-text-secondary">{title}</span>
		</div>
	</div>
</div>
