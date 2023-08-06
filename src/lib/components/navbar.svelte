<script>
	export let prop
	export let fixed
	let y;
</script>

<svelte:window bind:scrollY={y} />
<section
	class="max-w-[100vw] {prop==="other"||y > 20
		? 'text-white bg-[#070503]'
		: 'text-white   bg-zinc-900/40'} {fixed!=="true"?"fixed top-0 z-50":""} transition-all ease-in"
>
	<nav
		id="navbar"
		class="navbar  flex flex-row justify-between px-4 items-center p-1 "
	>
		<a href="/"><img src={y > 20 ? './vasista_white.png' : './vasista_white.png'} alt="logo" class="h-[60px]" /></a>
		<div class="flex flex-row items-center">
			<div class="hidden md:block">
				<a href={prop==="other"?"/#aboutus":"#aboutus"} class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
					>About Us</a
				>
				<a href="/enquiry" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
					>Enquiry</a
				>
				<a href="#contactus" class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
					>Contact Us</a
				>
				<a href="/gallery" class=" p-4 hover:underline underline-offset-4 ease-in transition-all"
					>Gallery</a
				>
			</div>
			<button
				class=" h-[40px] px-3 transition-all ease-in {y > 20
					? ' border-white hover:bg-white hover:text-black'
					: ' border-white hover:bg-white hover:text-black'} border-2 mx-2">Order Now</button
			>
		</div>
	</nav>

	<div class=" md:hidden text-sm flex flex-row justify-evenly w-[100vw] pb-2">
		<a href="#aboutus" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
			>About Us</a
		>
		<a href="/enquiry" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
			>Enquiry</a
		>
		<a href="#contactus" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
			>Contact Us</a
		>
		<a href="/gallery" class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
			>Gallery</a
		>
	</div>
</section>
