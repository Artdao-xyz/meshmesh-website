<script lang="ts">
	let formData = {
		fullName: '',
		email: '',
		businessName: '',
		description: ''
	};

	function handleSubmit(event: SubmitEvent) {
		event.preventDefault();
		// Form submission logic will go here
		console.log('Form submitted:', formData);
	}
</script>

<div class="bg-linear-to-b from-border-white to-[#929292] rounded-form p-[3px] w-full max-w-[890px] shadow-(--shadow-card) md:w-[890px]">
	<div class="bg-card-gray rounded-form px-6 py-8 md:p-9 w-full flex flex-col items-center gap-4 md:gap-form-container-gap">
		<div class="flex flex-col items-center gap-description-gap w-full">
			<h2 class="font-kabel font-black text-4xl md:text-6xl leading-[0.9] tracking-[-1.8px] text-text-primary text-center uppercase m-0 w-full md:tracking-[-3px] md:max-w-xl">
				<span class="hidden md:block">Early access drops </span>
				<span class="block md:hidden">Early access</span>
				<span class="block md:hidden">drops</span>
				<span>every Monday</span>
			</h2>
			<p class="font-sans font-normal leading-[1.4] text-text-primary text-center w-full m-0 whitespace-pre-wrap md:text-lg md:w-[669px]">
				Save your place and we'll send you an invite code by email to download MeshMesh Studio loaded with free credits.
			</p>
		</div>

		<form onsubmit={handleSubmit} class="flex flex-col items-center gap-[20px] md:gap-5 w-full">
			<div class="flex flex-col gap-inputs-gap md:gap-5 items-start w-full">
				<div class="flex flex-col gap-inputs-gap md:gap-inputs-gap w-full md:flex-row">
					<input
						type="text"
						placeholder="Full Name"
						bind:value={formData.fullName}
						class="flex-1 h-[40px] min-h-[40px] max-h-[40px] md:h-[47px] md:min-h-[47px] md:max-h-[47px] border-[0.6px] border-text-primary rounded-full pl-6 pr-2.5 font-sans font-normal text-lg leading-none text-text-primary bg-transparent outline-none placeholder:text-text-primary box-border"
						required
					/>
					<input
						type="email"
						placeholder="Email"
						bind:value={formData.email}
						class="flex-1 h-[40px] min-h-[40px] max-h-[40px] md:h-[47px] md:min-h-[47px] md:max-h-[47px] border-[0.6px] border-text-primary rounded-full pl-6 pr-2.5 font-sans font-normal text-lg leading-none text-text-primary bg-transparent outline-none placeholder:text-text-primary box-border"
						required
					/>
					<input
						type="text"
						placeholder="Business Name"
						bind:value={formData.businessName}
						class="flex-1 h-[40px] min-h-[40px] max-h-[40px] md:h-[47px] md:min-h-[47px] md:max-h-[47px] border-[0.6px] border-text-primary rounded-full pl-6 pr-2.5 font-sans font-normal text-lg leading-none text-text-primary bg-transparent outline-none placeholder:text-text-primary box-border"
						required
					/>
				</div>
				<div class="flex flex-col gap-4 md:gap-description-gap w-full">
					<p class="font-sans font-normal md:text-lg leading-[1.2] text-text-primary m-0 whitespace-pre-wrap mt-3 md:mt-0">
						Got Skills? Get paid bounties for use case validation, trailblazer feedback, & video testimonials.
					</p>
					<textarea
						placeholder="Description"
						bind:value={formData.description}
						rows="3"
						class="flex-1 border-[0.6px] border-text-primary rounded-textarea p-4 md:p-6 font-sans font-normal text-lg leading-[1.2] text-text-primary bg-transparent outline-none resize-y min-h-[50px] md:min-h-[100px] h-auto w-full placeholder:text-text-primary box-border"
					></textarea>
				</div>
			</div>
			<button
				type="submit"
				class="bg-text-primary border-[1.623px] border-bg-gray rounded-button px-[16.23px] py-[8.115px] h-[49.23px] w-[207.2px] font-mono font-medium text-lg leading-[1.2] tracking-[-0.18px] md:tracking-[-1px] text-bg-gray cursor-pointer uppercase hover:opacity-90"
			>
				SUBMIT
			</button>
		</form>
	</div>
</div>
