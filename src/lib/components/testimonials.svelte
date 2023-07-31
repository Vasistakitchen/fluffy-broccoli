<script>
	let reviews = [
		'I was thrilled with the unique charm of this small restaurant . I enjoyed exceptional flavors in the dishes and appreciated the attentive service. Excited to return and try more from the menu.',
		'The restaurant is a hidden gem, offering mouthwatering food, affordable prices, and excellent personalized service, making it highly recommended for a delightful dining experience.',
		'The restaurant is a hidden gem, offering mouthwatering food, affordable prices, and excellent personalized service, making it highly recommended for a delightful dining experience.'
	];
	let names = ['Naveen', 'Ravi', 'Shyam'];
</script>

<section class="  max-w-[1600px] mx-auto">
	<div class="flex flex-col p-8">
		<h1 class="text-3xl md:text-5xl p-4  text-gray-700 font-semibold text-center md:text-start">
			What our customers say
		</h1>


	<div
		data-aos="fade-up"
		class="testimonials grid grid-cols-1 gap-4  md:grid-cols-3 items-center my-2"
	>
		{#each Array(names.length) as _, index}
			<div data-aos="fade-up" data-aos-delay={(index + 1) * 100} class="basis-1/3">
				<div class="testimonial max-w-[400px] mx-auto flex flex-col items-start gap-2 p-4">
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
					<p class="text-gray-700 text-justify text-sm xl:text-xl">
						{reviews[index]}
					</p>
					<h1 class="font-bold my-2">- {names[index]}</h1>
				</div>
			</div>
		{/each}
	</div>
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
