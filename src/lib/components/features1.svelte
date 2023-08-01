<script>
	import Foodplate from './foodplate.svelte';
	import Dining from './dining.svelte';
	import Delivery from './delivery.svelte';
	import Catering from './catering.svelte';
</script>

<section class=" max-w-[1600px] mx-auto">
	<div class="  ">
		<div
			class=" grid sm:grid-cols-2 p-8 justify-center gap-4 align-middle items-center text-center"
		>
			<div data-aos="fade-up" class="   p-4 flex flex-col gap-2">
				<Foodplate />
				<p class=" text-left font-bold lg:text-xl mt-4">Wide range of menu</p>
				<p class="  font-normal text-justify text-sm lg:text-xl">
					Savor an array of delectable flavors from our wide-ranging menu, carefully curated to
					cater to every palate. Whether you crave classic favorites or adventurous dishes, we have
					something to delight everyone.
				</p>
			</div>
			<div data-aos="fade-up" class="   p-4 flex flex-col gap-2">
				<Dining />
				<p class=" text-left font-bold lg:text-xl mt-4">Open Garden Dining</p>
				<p class="  font-normal text-justify text-sm lg:text-xl">
					Indulge in a memorable dining experience amidst nature's beauty at our open garden
					setting. Enjoy delicious food while surrounded by a serene and charming ambiance.
				</p>
			</div>

			<div data-aos="fade-up" class="   p-4 flex flex-col gap-2">
				<Delivery />
				<p class=" text-left font-bold lg:text-xl mt-4">Door step delivery</p>
				<p class="  font-normal text-justify text-sm lg:text-xl">
					Experience the convenience of doorstep delivery, bringing our delectable cuisine straight
					to your home. Enjoy the same great taste and quality, now at your doorstep.
				</p>
			</div>
			<div data-aos="fade-up" class="   p-4 flex flex-col gap-2">
				<Catering />
				<p class=" text-left font-bold lg:text-xl mt-4">Corporate events and catering</p>
				<p class="  font-normal text-justify text-sm lg:text-xl">
					Elevate your events with our impeccable catering services, offering a culinary journey
					that impresses every guest. From small gatherings to large-scale events, we ensure a
					seamless and delightful dining experience.
				</p>
			</div>
		</div>
	</div>
</section>
