<script>
    import {enquiry} from "./store.js"
</script>
<div>
	<h1 class="py-2 font-bold">* Select type of enquiry</h1>
	<div class="flex gap-4 bg-slate-200 rounded-2xl p-4 max-w-[250px] justify-evenly">
		<div>
			<input on:change={()=>{
				let v = document.querySelector('input[name="tabs"]:checked').value
				$enquiry=v
				console.log($enquiry)
			}}
				type="radio"
				id="option0"
				name="tabs"
				checked="true"
				value="dining"
				class="peer/option1 appearance-none"
			/>
			<label
				for="option0"
				class="p-2 px-4 text-xl cursor-pointer font-bold rounded-xl peer-checked/option1:bg-gray-900 peer-checked/option1:text-gray-200"
				>Dining</label
			>
		</div>
		<div>
			<input on:change={()=>{
				let v = document.querySelector('input[name="tabs"]:checked').value
				$enquiry=v
				console.log($enquiry)
			}} type="radio" value="catering" id="option1" name="tabs" class="peer/option2 appearance-none" />
			<label
				for="option1"
				class="p-2 text-xl rounded-xl cursor-pointer font-bold peer-checked/option2:bg-gray-900 peer-checked/option2:text-gray-200"
				>Catering</label
			>
		</div>
	</div>
</div>
