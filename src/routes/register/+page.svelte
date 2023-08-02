
<script>
	import Navbar from '../../lib/components/navbar.svelte';
	import Footer from '../../lib/components/footer.svelte';
    import Register from "./components/register.svelte";
</script>

<section class=" text-gray-700 flex flex-col overflow-x-hidden justify-between grow h-[100vh]">
	<Navbar fixed="true" prop="other" />
	<div class="flex flex-row max-xl:justify-center flex-auto">
		<div class="image m-6 hidden flex-initial md:block min-w-[50%]" />
		<form class="md:w-[50%] max-w-[640px] min-w-[310px] 2xs:min-w-[350px] flex flex-col  gap-4 p-6 rounded-lg md:m-10">
			<h1 class="text-3xl font-bold">Register Here</h1>
			<Register/>
            <button class="max-w-[100px] py-2 text-gray-300 bg-gray-800 rounded-lg font-bold" >Submit</button>
		</form>
	</div>
	<Footer />
    
</section>

<style>
	.image {
		background: linear-gradient(180deg, rgba(27, 19, 24, 0.3), rgba(12, 4, 8, 0.425)),
			url('../../lib/images/enquiry.jpg');
		background-size:cover ;
	}
</style>
