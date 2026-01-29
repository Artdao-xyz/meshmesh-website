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
		<svg
			preserveAspectRatio="none"
			width="100%"
			height="100%"
			overflow="visible"
			style="display: block; shape-rendering: geometricPrecision;"
			viewBox="0 0 102.941 102.941"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<g id="Play-button" filter="url(#filter0_d_1192_8849)">
				<rect
					x="16.4706"
					y="16.4706"
					width="70"
					height="70"
					rx="16.4706"
					fill="var(--fill-0, #D7D7D7)"
					style="shape-rendering: geometricPrecision;"
				/>
				<rect
					x="17.7059"
					y="17.7059"
					width="67.5294"
					height="67.5294"
					rx="15.2353"
					stroke="url(#paint0_linear_1192_8849)"
					stroke-width="2.47059"
					style="shape-rendering: geometricPrecision;"
				/>
				<path
					id="Polygon 1 (Stroke)"
					d="M64.7593 49.8344C65.9967 50.5616 65.9967 52.3796 64.7592 53.1068L44.1558 65.2146C42.957 65.9191 41.4678 65.0881 41.3759 63.7132L41.3715 63.5785L41.3715 39.3627C41.3715 37.9083 42.9183 36.9993 44.1558 37.7265L64.7593 49.8344Z"
					fill="var(--fill-0, #272727)"
				/>
			</g>
			<defs>
				<filter
					id="filter0_d_1192_8849"
					x="0"
					y="0"
					width="102.941"
					height="102.941"
					filterUnits="userSpaceOnUse"
					color-interpolation-filters="sRGB"
				>
					<feFlood flood-opacity="0" result="BackgroundImageFix" />
					<feColorMatrix
						in="SourceAlpha"
						type="matrix"
						values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
						result="hardAlpha"
					/>
					<feOffset />
					<feGaussianBlur stdDeviation="8.23529" />
					<feComposite in2="hardAlpha" operator="out" />
					<feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.2 0" />
					<feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_1192_8849" />
					<feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_1192_8849" result="shape" />
				</filter>
				<linearGradient
					id="paint0_linear_1192_8849"
					x1="51.4706"
					y1="16.4706"
					x2="51.4706"
					y2="86.4706"
					gradientUnits="userSpaceOnUse"
				>
					<stop stop-color="#F9F9F9" />
					<stop offset="1" stop-color="#939393" />
				</linearGradient>
			</defs>
		</svg>
	</div>
</button>
