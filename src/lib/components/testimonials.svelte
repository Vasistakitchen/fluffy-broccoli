

<section class=" lg:w-[90vw] max-w-[1600px] mx-auto">
	<div class="testimonials grid grid-cols-1  md:grid-cols-3 items-center my-2">
		<div class="basis-1/3">
			<div class="text-center p-4 mx-auto max-w-[400px]  text-5xl font-bold text-gray-700 my-2">
				What our customers say
			</div>
		</div>
		{#each Array(2) as _, index}
			<div class="basis-1/3">
				<div
					class="testimonial max-w-[400px] mx-auto max-md:min-w-[310px]  flex flex-col items-start gap-2 p-8"
				>
					<svg
						class="h-8 fill-gray-600"
						style="shape-rendering:geometricPrecision;text-rendering:geometricPrecision;image-rendering:optimizeQuality;"
						viewBox="0 0 100000 125000"
						x="0px"
						y="0px"
						fill-rule="evenodd"
						clip-rule="evenodd"
						><defs
							><style type="text/css">
							</style></defs
						><g
							><path
								class="fil0"
								d="M38287 85139l0 -35139 -23426 0c0,-12913 10501,-23426 23426,-23426l0 -11713c-19375,0 -35139,15763 -35139,35139l0 35139 35139 0z"
							/><path
								class="fil0"
								d="M96852 85139l0 -35139 -23426 0c0,-12913 10501,-23426 23428,-23426l0 -11713c-19377,0 -35140,15763 -35140,35139l0 35139 35138 0z"
							/></g
						></svg
					>
					<p class="text-gray-700 text-justify text-sm">
						Excepteur exercitation mollit exercitation irure in consectetur minim laboris cupidatat
						labore cupidatat eu Lorem. Magna nulla voluptate quis mollit cillum ut cupidatat amet
						eiusmod duis.
					</p>
					<h1 class="font-bold my-2">- Naveen</h1>
				</div>
			</div>
		{/each}
	</div>
</section>

<style>
	.testimonials {
		font-family: nexa;
	}

	.testimonials {
		scrollbar-width: thin;
		scrollbar-color: #f2933a #ffffff;
	}

	.testimonials::-webkit-scrollbar {
		width: 10px;
	}

	.testimonials::-webkit-scrollbar-track {
		background: #ffffff;
	}

	.testimonials::-webkit-scrollbar-thumb {
		background-color: #f2933a;
		border-radius: 10px;
		border: 3px solid #ffffff;
	}
</style>
