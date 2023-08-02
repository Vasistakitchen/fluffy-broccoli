<input
	required
	type="text"
	class="bg-gray-100 p-2 px-4 placeholder:font-bold font-bold tracking-wider rounded-md"
	placeholder="Name"
    name="name"
/>
<input
	required
	type="number"
	class="bg-gray-100 p-2 px-4 placeholder:font-bold font-bold tracking-wider rounded-md"
	placeholder="+91 95xxx xxx58"
    name="number"
/>
<input
	required
	type="number"
	class="bg-gray-100 p-2 px-4 placeholder:font-bold font-bold tracking-wider rounded-md"
	placeholder="whats app number"
    name="wh_number"
/>
<h6 class="text-xl font-semibold">Food you like</h6>
<div class="flex items-center ">
	<input class="appearance-none peer/veg" type="checkbox" id="indian" value="indian" name="typeofcusine" />
	<label class="border cursor-pointer border-gray-800 peer-checked/veg:bg-gray-600 peer-checked/veg:text-gray-300 font-bold px-4 py-1 rounded-full " for="indian">Indian</label>
	<input class="appearance-none peer/italian" type="checkbox" id="italian" value="nonveg" name="typeofcusine" />
	<label class="border cursor-pointer border-gray-800 peer-checked/italian:bg-gray-600 peer-checked/italian:text-gray-300 font-bold px-4 ml-4 py-1 rounded-full " for="italian">Italian</label>
    <input class="appearance-none peer/chainees" type="checkbox" id="chainees" value="nonveg" name="typeofcusine" />
	<label class="border cursor-pointer border-gray-800 peer-checked/chainees:bg-gray-600 peer-checked/chainees:text-gray-300 font-bold px-4 ml-4 py-1 rounded-full " for="chainees">chainees</label>

</div>


