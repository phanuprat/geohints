<script>
	import '../app.css';
	import Nav from "../components/Nav.svelte";
</script>

<div>
	<div class="min-h-screen overflow-x-hidden bg-[#14151a]">
		<Nav/>
		<slot />
	</div>
</div>
