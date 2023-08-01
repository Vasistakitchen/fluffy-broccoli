<script>
	import Navbar from '../../lib/components/navbar.svelte';
	import Footer from '../../lib/components/footer.svelte';
</script>

<section class=" text-gray-700 flex flex-col  justify-between grow h-[100vh]">
	<Navbar fixed="true" prop="other" />
	<div class="flex flex-row max-xl:justify-center flex-auto">
		<div class="image hidden flex-initial md:block min-w-[50%]" />
		<form class="md:w-[50%] max-w-[640px] min-w-[310px] 2xs:min-w-[350px] flex flex-col  gap-4 p-6 rounded-lg md:m-10">
			<h1 class="text-3xl font-bold">Enquiry form</h1>
			<div>
				<h1 class="py-2 font-bold">* Select type of enquiry</h1>
				<div class="flex gap-4 bg-slate-200 rounded-2xl p-4 max-w-[250px] justify-evenly">
					<div>
						<input
							type="radio"
							id="option0"
							name="tabs"
							checked="true"
							class="peer/option1 appearance-none"
						/>
						<label
							for="option0"
							class="p-2 px-4 text-xl font-bold rounded-xl peer-checked/option1:bg-gray-900 peer-checked/option1:text-gray-200"
							>Dining</label
						>
					</div>
					<div>
						<input type="radio" id="option1" name="tabs" class="peer/option2 appearance-none" />
						<label
							for="option1"
							class="p-2 text-xl rounded-xl font-bold peer-checked/option2:bg-gray-900 peer-checked/option2:text-gray-200"
							>Catering</label
						>
					</div>
				</div>
			</div>
			<input
				required
				type="text"
				class="bg-gray-100 p-2 px-4 placeholder:font-bold font-bold tracking-wider rounded-md"
				placeholder="Name"
			/>
			<input
				required
				type="number"
				class="bg-gray-100 p-2 px-4 placeholder:font-bold font-bold tracking-wider rounded-md"
				placeholder="+91 95xxx xxx58"
			/>
			<input
				required
				type="date"
				class="bg-gray-100 p-2 px-4  font-bold tracking-wider rounded-md"
				
			/>
			<input
				required
				type="time"
				class="bg-gray-100 p-2 px-4  font-bold tracking-wider rounded-md"
				
			/>
            <input
				required
				type="number"
				class="bg-gray-100 p-2 px-4 placeholder:font-bold font-bold tracking-wider rounded-md"
				placeholder="Total no.of persons"
			/>
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
