<script>
	import Carousel from '../components/Carousel.svelte';
	
	let colors = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
</script>

<div class="relative w-full px-4 py-4">
	<!---->
	<section
		class="w-full px-8 md:px-12 xl:max-w-7xl mx-auto lg:px-7 xl:px-10 bg-[#1d1e23] lg:mt-24 p-6 rounded-[40px] text-white"
	>
	<Carousel controls>

		<!-- Meta Carousel -->
			<div class="relative h-auto p-6 rounded-3xl bg-[#112f44] mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/alphabet.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Alphabet</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#10233a] mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/road.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Road</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#3dc9e0] mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/sign.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Signs</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-blue-500 mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/architecture.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Architecture</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#5b4a37] mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/flag.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Flags</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#5cc6b6] mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/utility-pole.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Utility pole</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-orange-500 mr-4">
				<img class="w-1/3 sm:w-4/5 mx-auto pb-12" src="/assets/img/dribbble_nd-transformed.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">License plate</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-red-500 mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/tree.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Nature</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-emerald-500 mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="/assets/img/hint/website.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Domain</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-pink-500 mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="https://cdn-icons-png.flaticon.com/512/3095/3095141.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Scenery</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-purple-500 mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="https://cdn-icons-png.flaticon.com/512/3267/3267422.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Traffic Lights</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-amber-100 mr-4">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="https://cdn-icons-png.flaticon.com/512/3267/3267422.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Something</h1>
			</div>
		</Carousel>


		<!-- <div class="w-full grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-x-6 gap-y-4 mt-4 gopher mb-8">
			<div class="relative h-auto p-6 rounded-3xl bg-[#112f44]">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/alphabet.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Alphabet</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#10233a]">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/road.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Road</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#3dc9e0]">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/sign.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Signs</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-blue-500">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/architecture.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Architecture</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#5b4a37]">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/flag.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Flags</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-[#5cc6b6]">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/utility-pole.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Utility pole</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-orange-500">
				<img class="w-1/3 sm:w-4/5 mx-auto pb-12" src="/assets/img/dribbble_nd-transformed.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">License plate</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-red-500">
				<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/tree.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Nature</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-emerald-500">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="/assets/img/hint/website.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Domain</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-pink-500">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="https://cdn-icons-png.flaticon.com/512/3095/3095141.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Scenery</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-purple-500">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="https://cdn-icons-png.flaticon.com/512/3267/3267422.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Traffic Lights</h1>
			</div>
			<div class="relative h-auto p-6 rounded-3xl bg-amber-100">
				<img class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4" src="https://cdn-icons-png.flaticon.com/512/3267/3267422.png">
				<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Something</h1>
			</div>
		</div> -->
	</section>
	
</div>