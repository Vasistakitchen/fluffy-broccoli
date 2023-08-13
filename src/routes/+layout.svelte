<script>
  import "./styles.css";
	import { onMount } from "svelte";
	import aos from "aos/dist/aos";
	import 'aos/dist/aos.css'; // You can also use <link> for styles



  onMount(()=>{
    aos.init({
      // once:true
    })
  })
</script>
<slot />