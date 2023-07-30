<script>
	let y;
</script>

<svelte:window bind:scrollY={y}  />
<section class="{y > 20
	? 'text-white bg-[#070503]'
	: 'text-white   bg-zinc-900/40'} fixed top-0 z-50 transition-all ease-in ">
<nav
	id="navbar"
	class="navbar  w-[100vw]  flex flex-row justify-around items-center p-2 mb-2 "
>
	<img src={y > 20 ? './vasista_white.png' : './vasista_white.png'} alt="logo" class="h-[60px]" />
	<div class="hidden md:block">
		<a href="#" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>About Us</a
		>
		<a href="#" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Enquiry</a
		>
		<a href="#" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Contact Us</a
		>
	</div>
	<button
		class=" h-[40px] px-4 transition-all ease-in {y > 20
			? ' border-white hover:bg-white hover:text-black'
			: ' border-white hover:bg-white hover:text-black'} border-2 mx-2">Order Now</button
	>
</nav>

<div
	class=" md:hidden  text-sm   flex flex-row justify-evenly  w-[100vw] pb-2"
>
	<a href="#" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
		>About Us</a
	>
	<a href="#" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
		>Enquiry</a
	>
	<a href="#" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
		>Contact Us</a
	>
</div>
</section>