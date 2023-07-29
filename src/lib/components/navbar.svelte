<script>
	let y;
</script>

<svelte:window bind:scrollY={y}  />
<nav
	id="navbar"
	class="navbar transition-all ease-in {y > 20
		? 'text-black bg-slate-100'
		: 'text-white   bg-zinc-900/40'} w-[100vw] z-50 flex flex-row justify-around items-center p-2 mb-2 fixed top-0"
>
	<img src={y > 20 ? './vasista_black.png' : './vasista_white.png'} alt="logo" class="h-[60px]" />
	<div class="hidden md:block">
		<a href="#/" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Browse Menu</a
		>
		<a href="#/" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Service Request</a
		>
		<a href="#/" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Contact Us</a
		>
	</div>
	<button
		class=" h-[40px] px-4 transition-all ease-in {y > 20
			? ' border-black hover:bg-black hover:text-white'
			: ' border-white hover:bg-white hover:text-black'} border-2 mx-2">Order Now</button
	>
</nav>

<div
	class="fixed md:hidden z-50 text-sm transition-all ease-in {y > 20
		? 'text-black  bg-slate-100'
		: 'text-white   bg-zinc-900/40'} top-[76px] flex flex-row justify-evenly bg-zinc-900/40 w-[100vw] pb-2"
>
	<a href="#/" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
		>Browse Menu</a
	>
	<a href="#/" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
		>Service Request</a
	>
	<a href="#/" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
		>Contact Us</a
	>
</div>
