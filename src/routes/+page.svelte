<script lang="ts">
	import EarlyAccessForm from '$lib/components/EarlyAccessForm.svelte';
	import TestimonialCard from '$lib/components/TestimonialCard.svelte';
</script>

<div class="relative w-full min-h-screen bg-bg-gray overflow-x-hidden font-suisse">
	<!-- Background Image -->
	<div class="absolute left-0 top-0 w-full h-screen overflow-hidden pointer-events-none z-0">
		<img src="/image-background.png" alt="Background" class="absolute w-full h-full object-cover left-0 top-0" />
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
				<p class="font-normal text-lg leading-[1.4] text-text-hero text-center w-full m-0 whitespace-pre-wrap md:text-2xl md:w-[755px]">
					See how Salesforce admins are cutting 90% time, doing it themselves, with no developer needed. Early access is open.
					<br />
					Comes with a sandbox to try it for free.
				</p>
			</div>
		</div>
	</section>

	<!-- Second Screen - Form Section -->
	<section id="form-section" class="relative w-full max-w-[1440px] mx-auto flex flex-col items-center gap-10 md:gap-form-gap py-hero-padding-y px-5 z-10 md:px-hero-padding-x">
		<EarlyAccessForm />

		<!-- Testimonials Section -->
		<div class="-translate-x-3.5 md:translate-x-0 w-full overflow-x-auto md:overflow-x-visible py-4 md:py-0 p-4">
			<div class="flex flex-row gap-[30px] w-max md:w-full md:flex-row md:flex-wrap md:justify-center">
				<TestimonialCard
					quote='"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt."'
					name="First Name"
					title="Title"
				/>
				<TestimonialCard
					quote='"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt."'
					name="First Name"
					title="Title"
				/>
				<TestimonialCard
					quote='"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt."'
					name="First Name"
					title="Title"
				/>
			</div>
		</div>
	</section>
</div>
