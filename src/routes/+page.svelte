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

	function scrollToForm() {
		const form = document.getElementById('form-section');
		form?.scrollIntoView({ behavior: 'smooth' });
	}
</script>

<div class="relative w-full min-h-screen bg-bg-gray overflow-x-hidden">
	<!-- Background Image -->
	<div class="absolute left-0 top-0 w-full h-screen overflow-hidden pointer-events-none z-0">
		<img src="/image-background.png" alt="Background" class="absolute w-full h-full object-cover object-[center_bottom] left-0 top-0" />
	</div>

	<!-- First Screen - Hero Section -->
	<section class="relative w-full h-screen flex flex-col items-center justify-between py-hero-padding-y pb-10 z-10 max-w-[1440px] mx-auto px-5 md:px-0">
		<div class="flex flex-col items-center gap-[30px] w-full">
			<div class="flex flex-col items-center gap-5 w-full md:gap-[30px]">
				<div class="h-10 w-[180px] relative md:h-[55.279px] md:w-[253.058px]">
					<img src="/logo-meshmesh.svg" alt="MeshMesh Logo" class="w-full h-full block" />
				</div>
				<h1 class="font-kabel font-black text-[48px] leading-[0.85] tracking-[-2px] text-text-hero text-center uppercase m-0 whitespace-pre-wrap max-w-[1030px] md:text-[95px] md:tracking-[-4px] md:leading-[0.79]">
					<span>Easy mode for </span>
					<span>Salesforce admins</span>
				</h1>
				<p class="font-sans font-normal text-lg leading-[1.4] text-text-hero text-center w-full px-5 m-0 whitespace-pre-wrap md:text-2xl md:w-[755px] md:px-0">
					See how Salesforce admins are cutting 90% time, doing it themselves, with no developer needed. Early access is open.
					<br />
					Comes with a sandbox to try it for free.
				</p>
			</div>
			<button
				onclick={scrollToForm}
				aria-label="Scroll to form"
				class="w-[58px] h-[58px] bg-transparent border-0 cursor-pointer p-0 block absolute bottom-5 left-1/2 -translate-x-1/2 shrink-0 z-20 md:bottom-10"
			>
				<img src="/icon-arrow.svg" alt="Scroll down" class="w-full h-full block" />
			</button>
		</div>
	</section>

	<!-- Second Screen - Form Section -->
	<section id="form-section" class="relative w-full max-w-[1440px] mx-auto flex flex-col items-center gap-form-gap py-hero-padding-y px-5 z-10 md:px-hero-padding-x">
		<div class="bg-card-gray border-[3px] border-border-white rounded-form p-9 w-full max-w-[890px] flex flex-col items-center gap-form-container-gap shadow-shadow-card md:w-[890px]">
			<div class="flex flex-col items-center gap-description-gap w-full">
				<h2 class="font-kabel font-black text-[36px] leading-[0.9] tracking-[-3px] text-text-primary text-center uppercase m-0 whitespace-pre-wrap w-full md:text-[60px] md:max-w-xl">
					Early access drops every Monday
				</h2>
				<p class="font-sans font-normal text-lg leading-[1.4] text-text-primary text-center w-full m-0 whitespace-pre-wrap md:text-2xl md:w-[669px]">
					Save your place and we'll send you an invite code by email to download MeshMesh Studio loaded with free credits.
				</p>
			</div>

			<form onsubmit={handleSubmit} class="flex flex-col items-center gap-5 w-full">
				<div class="flex flex-col gap-5 items-start w-full">
					<div class="flex flex-col gap-inputs-gap w-full md:flex-row">
						<input
							type="text"
							placeholder="Full Name"
							bind:value={formData.fullName}
							class="flex-1 h-[47px] border-[0.6px] border-text-primary rounded-full pl-6 pr-2.5 font-sans font-normal text-lg leading-[1.2] text-text-primary bg-transparent outline-none placeholder:text-text-primary"
							required
						/>
						<input
							type="email"
							placeholder="Email"
							bind:value={formData.email}
							class="flex-1 h-[47px] border-[0.6px] border-text-primary rounded-full pl-6 pr-2.5 font-sans font-normal text-lg leading-[1.2] text-text-primary bg-transparent outline-none placeholder:text-text-primary"
							required
						/>
						<input
							type="text"
							placeholder="Business Name"
							bind:value={formData.businessName}
							class="flex-1 h-[47px] border-[0.6px] border-text-primary rounded-full pl-6 pr-2.5 font-sans font-normal text-lg leading-[1.2] text-text-primary bg-transparent outline-none placeholder:text-text-primary"
							required
						/>
					</div>
					<div class="flex flex-col gap-description-gap w-full">
						<p class="font-sans font-normal text-lg leading-[1.2] text-text-primary m-0 whitespace-pre-wrap">
							Got Skills? Get paid bounties for use case validation, trailblazer feedback, & video testimonials.
						</p>
						<textarea
							placeholder="Description"
							bind:value={formData.description}
							rows="4"
							class="flex-1 border-[0.6px] border-text-primary rounded-textarea p-6 font-sans font-normal text-lg leading-[1.2] text-text-primary bg-transparent outline-none resize-y min-h-[100px] w-full placeholder:text-text-primary"
						></textarea>
					</div>
				</div>
				<button
					type="submit"
					class="bg-text-primary border-[1.623px] border-bg-gray rounded-button px-[16.23px] py-[8.115px] h-[49.23px] w-[207.2px] font-mono font-medium text-lg leading-[1.2] tracking-[-1px] text-bg-gray cursor-pointer uppercase hover:opacity-90"
				>
					SUBMIT
				</button>
			</form>
		</div>

		<!-- Testimonials Section -->
		<div class="flex flex-col gap-[30px] w-full justify-center md:flex-row md:flex-wrap">
			<div class="bg-card-gray border-[3px] border-border-white rounded-form px-10 py-9 w-full max-w-[430px] h-[250px] flex flex-col gap-form-container-gap shadow-shadow-card md:w-[430px]">
				<div class="flex-1 flex flex-col items-center w-full">
					<p class="font-sans font-normal text-2xl leading-[1.4] text-text-primary text-center m-0 whitespace-pre-wrap w-full">
						"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt."
					</p>
				</div>
				<div class="flex justify-between items-start w-full font-mono font-medium text-lg leading-[1.2] tracking-[-1px] text-center whitespace-nowrap">
					<span class="text-text-primary">First Name</span>
					<span class="text-text-secondary">Title</span>
				</div>
			</div>
			<div class="bg-card-gray border-[3px] border-border-white rounded-form px-10 py-9 w-full max-w-[430px] h-[250px] flex flex-col gap-form-container-gap shadow-shadow-card md:w-[430px]">
				<div class="flex-1 flex flex-col items-center w-full">
					<p class="font-sans font-normal text-2xl leading-[1.4] text-text-primary text-center m-0 whitespace-pre-wrap w-full">
						"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt."
					</p>
				</div>
				<div class="flex justify-between items-start w-full font-mono font-medium text-lg leading-[1.2] tracking-[-1px] text-center whitespace-nowrap">
					<span class="text-text-primary">First Name</span>
					<span class="text-text-secondary">Title</span>
				</div>
			</div>
			<div class="bg-card-gray border-[3px] border-border-white rounded-form px-10 py-9 w-full max-w-[430px] h-[250px] flex flex-col gap-form-container-gap shadow-shadow-card md:w-[430px]">
				<div class="flex-1 flex flex-col items-center w-full">
					<p class="font-sans font-normal text-2xl leading-[1.4] text-text-primary text-center m-0 whitespace-pre-wrap w-full">
						"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt."
					</p>
				</div>
				<div class="flex justify-between items-start w-full font-mono font-medium text-lg leading-[1.2] tracking-[-1px] text-center whitespace-nowrap">
					<span class="text-text-primary">First Name</span>
					<span class="text-text-secondary">Title</span>
				</div>
			</div>
		</div>
	</section>
</div>
