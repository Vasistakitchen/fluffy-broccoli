<script>
	let nav 
	let nav2 
	let y;
 function colornav() { 
	console.log(y)
    if (y >= 20 ) {
        nav.classList.add("bg-neutral-950");
        nav.classList.remove("bg-zinc-900/40");
        nav2.classList.add("bg-neutral-950");
        // nav2.classList.add("border-b-2 border-[#e29d07]");
        nav2.classList.remove("bg-zinc-900/40");
		console.log("hello")
    } 
    else {
        nav.classList.add("bg-zinc-900/40");
		nav.classList.remove("bg-neutral-950");
        nav2.classList.add("bg-zinc-900/40");
		nav2.classList.remove("bg-neutral-950");
       console.log("hy")
    }
};
</script>
<svelte:window bind:scrollY={y} on:scroll={colornav}/>
<nav bind:this={nav}
	id="navbar" class="navbar  text-white z-50 bg-zinc-900/40 w-[100vw] flex flex-row justify-between items-center p-2 mb-2 fixed top-0"
>
	<img src="./vasista_white.png" alt="logo" class="h-[60px]" />
	<div class="hidden md:block">
		<a
			href="#ntng"
			class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Browse Menu</a
		>
		<a
			href="#ntng"
			class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Service Request</a
		>
		<a
			href="#ntng"
			class=" p-4 hover:underline underline-offset-4 ease-in transition-all mx-2"
			>Contact Us</a
		>
	</div>
	<button
		class=" h-[40px] px-4  border-white hover:bg-white hover:text-black border-2 mx-2"
		>Order Now</button
	>
	
</nav>

<div bind:this={nav2} class="fixed md:hidden z-50 text-sm text-white top-[76px] flex flex-row justify-evenly bg-zinc-900/40 w-[100vw]  pb-2 ">
    <a
        href="#ntng"
        class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
        >Browse Menu</a
    >
    <a
        href="#ntng"
        class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
        >Service Request</a
    >
    <a
        href="#ntng"
        class=" p-2 hover:underline underline-offset-4 ease-in transition-all mx-1"
        >Contact Us</a
    >
</div>