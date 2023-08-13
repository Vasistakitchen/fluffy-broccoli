<script>
	import { onMount } from 'svelte';
	import { fade } from 'svelte/transition';
	let ready = false;
	
	onMount(() => (ready = true));
</script>

<section
	class="hero cursor-default overflow-hidden bg-gray-950 max-h-[550px] md:max-h-[600px] h-[100vh] bg-cover bg-center flex flex-col justify-center items-center"
>
	<div class="welcome-text flex flex-col relative">
		{#if ready}
		<h1
			transition:fade={{ delay: 250, duration: 300 }}
			class=" welcome text-3xl md:text-5xl text-center relative top-5 md:top-10 right-[0rem] text-slate-100"
		>
			Welcome to
		</h1>
		{/if}
		{#if ready}
		<h1
			transition:fade={{ delay: 450, duration: 300 }}
			class="vasista text-[#e29d07] text-[6rem] 2xs:text-[6.5rem] sm:text-[9rem] md:text-[11rem] z-0 font-extralight"
		>
			Vasista
		</h1>
		{/if}
		<!-- <h1 class="kitchen text-[#f3de9d] text-[11rem] z-0  relative bottom-48 right-[-10rem] font-extralight">Kitchen</h1> -->
	</div>
	<div class="flex justify-between relative z-10 items-center">
		{#if ready}
		<button transition:fade={{ delay: 650, duration: 300 }}
		class="text-white text-sm md:text-xl md:mt-[-30px] transition-all ease-in origin-right hover:bg-white hover:text-black border-white border-2 p-4"
		>Explore Kitchen</button
	>
		{/if}
		<!-- <a href="#menu" class="text-[#ffffff] p-4 mx-4 text-3xl hover:bg-white hover:text-black ">Browse Menu</a> -->
	</div>
</section>

<style>
	.hero {
		background: linear-gradient(180deg, rgba(27, 19, 24, 0.3), rgba(12, 4, 8, 0.425)),
			url('../images/food.jpg');
		background-size: cover;
	}
	
	@font-face {
		font-family: 'rylan';
		src: url('../fonts/Rylan-Regular.otf') format('opentype');
	}
	@font-face {
		font-family: 'jitter';
		src: url('../fonts/Jitter.otf') format('opentype');
	}
	@font-face {
		font-family: 'violitta';
		src: url('../fonts/Violitta.otf') format('opentype');
	}
	.vasista {
		font-family: rylan;
	}
	.welcome {
		font-family: jitter;
	}
	/* .kitchen{
		font-family: violitta;
	} */


</style>
