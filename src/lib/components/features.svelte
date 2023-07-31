<script>
	let headings = [
		'Wide range of menu',
		'Open garden dining',
		'Door step delivery',
		'Events & catering'
	];
	let descriptions = [
		'Savor an array of delectable flavors from our wide-ranging menu, carefully curated to cater to every palate. Whether you crave classic favorites or adventurous dishes, we have something to delight everyone.',
		"Indulge in a memorable dining experience amidst nature's beauty at our open garden setting. Enjoy delicious food while surrounded by a serene and charming ambiance.",
		'Experience the convenience of doorstep delivery, bringing our delectable cuisine straight to your home. Enjoy the same great taste and quality, now at your doorstep.',
		'Elevate your events with our impeccable catering services, offering a culinary journeythat impresses every guest. From small gatherings to large-scale events, we ensure aseamless and delightful dining experience.'
	];
	let icons = [
		'./fast-food-outline.svg',
		'./restaurant.svg',
		'./door-closed.svg',
		'./concierge-bell.svg'
	];
</script>

<section class="max-w-[1600px] mx-auto text-gray-700">
	<div class="flex flex-col p-8">
		<h1 class="text-4xl md:text-5xl p-4 text-gray-700 font-semibold text-center md:text-start">
			What we provide
		</h1>

		<div  class="features p-4 grid md:grid-cols-2 lg:grid-cols-4 justify-items-center gap-4">
			{#each Array(headings.length) as _, index}
				<div data-aos="fade-up" data-aos-delay={index*100} class="feature bg-slate-100 hover:scale-[1.02] ease-in transition-all p-6 flex flex-col gap-3 max-w-[360px] rounded-xl">
					<div class="flex flex-row items-center gap-2">
						<img src={icons[index]} class="h-8" alt="food" />
						<p class=" text-left font-bold text-xl">{headings[index]}</p>
					</div>
					<p class="  font-normal">
						{descriptions[index]}
					</p>
				</div>
			{/each}
		</div>
	</div>
</section>
