<script>
	import Hint from '../components/Hint.svelte';
	const forceUpdate = async (_) => {};
	let doRerender = 0;
	$: innerWidth = 0;
	let perPage = 0;
	function resize() {
		if (innerWidth >= 380 && innerWidth < 640) {
			perPage = 1;
		}
		if (innerWidth >= 640 && innerWidth < 768) {
			perPage = 2;
		}
		if (innerWidth >= 768 && innerWidth < 1024) {
			perPage = 4;
		}
		if (innerWidth > 1024) {
			perPage = 6;
		}
		if (innerWidth < 380) {
			perPage = 1;
		}
	}
	function checkscreensize() {
		if (innerWidth === 0) {
			setTimeout(resize, 100);
			setTimeout(() => doRerender++, 100);
		} else {
			resize();
		}
	}
</script>

<svelte:window bind:innerWidth on:resize={resize} on:resize={checkscreensize} on:resize={() => doRerender++} />

{#await innerWidth then innerWidth}
	<div class="hidden">{checkscreensize()}</div>
{/await}

<div class="relative w-full px-4 py-4">
	<!---->
	<section
		class="w-full px-8 md:px-12 xl:max-w-7xl mx-auto lg:px-7 xl:px-10 bg-[#1d1e23] lg:mt-24 pt-6 pb-2 rounded-[20px] text-white"
	>
		{#await forceUpdate(doRerender) then _}
			{#await perPage}
			{:then perPage}
				<Hint controls {perPage}>
					<!-- Meta Carousel -->
					<div class="relative h-auto p-6 rounded-3xl bg-[#112f44] mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto pb-12"
							src="/assets/img/hint/alphabet.png"
							alt="Alphabet"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Alphabet</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-[#10233a] mr-4">
						<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/road.png" alt="Road" />
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Road</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-cyan-500 mr-4">
						<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/sign.png" alt="Signs" />
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Signs</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-sky-500 mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto pb-12"
							src="/assets/img/hint/architecture.png"
							alt="Architecture"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Architecture</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-[#5b4a37] mr-4">
						<img class="w-1/3 sm:w-3/5 mx-auto pb-12" src="/assets/img/hint/flag.png" alt="Flags" />
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Flags</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-[#5cc6b6] mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto pb-12"
							src="/assets/img/hint/utility-pole.png"
							alt="Utility pole"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Utility pole</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-orange-500 mr-4">
						<img
							class="w-1/3 sm:w-4/5 mx-auto pb-12"
							src="/assets/img/dribbble_nd-transformed.png"
							alt="License plate"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">License plate</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-red-500 mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto pb-12"
							src="/assets/img/hint/tree.png"
							alt="Nature"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Nature</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-emerald-500 mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg mt-4 pb-3"
							src="/assets/img/hint/website.png"
							alt="Domain"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Domain</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-pink-500 mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg"
							src="/assets/img/hint/scenery.png"
							alt="Scenery"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Scenery</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-purple-500 mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg"
							src="https://cdn-icons-png.flaticon.com/512/3267/3267422.png"
							alt="Traffic Lights"
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Traffic Lights</h1>
					</div>
					<div class="relative h-auto p-6 rounded-3xl bg-blue-500 mr-4">
						<img
							class="w-1/3 sm:w-3/5 mx-auto mb-12 rounded-lg"
							src="https://cdn-icons-png.flaticon.com/512/3267/3267422.png"
							alt=""
						/>
						<h1 class="text-2xl md:text-xl font-bold absolute bottom-6 left-6">Something</h1>
					</div>
				</Hint>
			{/await}
		{/await}
</div>
