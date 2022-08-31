<header>
	<input type="checkbox" name="hbr" id="hbr" class="hbr peer" hidden aria-hidden="true" />
	<nav
		class="z-10 w-full navbar peer-checked:navbar-active md:absolute bg-transparent"
	>
		<div class="container m-auto px-2 md:px-12 lg:px-7">
			<div class="flex flex-wrap items-center justify-between gap-6 md:py-3 md:gap-0">
				<div class="w-full px-6 flex justify-between lg:w-max md:px-0 pt-4">
					<a href="#" aria-label="logo" class="flex space-x-2 items-center">
						<img class="h-10" src="https://www.geoguessr.com/_next/static/images/logo-dd3c3286e6d14f72653800dbdf5340a0.svg">
					</a>
					<label
						for="hbr"
						class="peer-checked:hamburger block relative z-20 p-6 -mr-6 cursor-pointer lg:hidden"
					>
						<div
							aria-hidden="true"
							class="m-auto h-0.5 w-6 rounded bg-sky-900 transition duration-300"
						/>
						<div
							aria-hidden="true"
							class="m-auto mt-2 h-0.5 w-6 rounded bg-sky-900 transition duration-300"
						/>
					</label>
				</div>
				<div
					class="navmenu hidden w-full flex-wrap justify-end items-center mb-16 mx-6 space-y-20 p-6 rounded-xl shadow-lg bg-white lg:space-y-0 lg:p-0 lg:m-0 lg:flex md:flex-nowrap lg:bg-transparent lg:w-7/12 lg:shadow-none"
				>
					<div class="text-cyan-600 lg:pr-4">
						<ul
							class="space-y-6 space-x-3 tracking-wide font-medium text-lg lg:text-sm lg:flex lg:space-y-0"
						>
							<!-- <li>
								<button class="bg-main text-white py-3 px-6 rounded-lg"> Contact Us </button>
							</li> -->
							<li>
								<button class="bg-main text-white py-3 px-6 rounded-lg flex items-center">
									<img class="mr-2" src="https://www.geoguessr.com/static/flags/US.svg" />
									English
								</button>
							</li>
							<li>
								<button
									class="bg-gradient-to-tr from-[#85d05b] to-[#78bb4b] text-white py-3 px-6 rounded-lg"
								>
									Donate
								</button>
							</li>
						</ul>
					</div>
				</div>
			</div>
		</div>
	</nav>
</header>

<style>
	.navbar-active .hamburger div:first-child {
		@apply rotate-45 translate-y-1.5;
	}
	.navbar-active .hamburger div:last-child {
		@apply -rotate-45 -translate-y-1;
	}
	.navbar-active div:first-child div:first-child div:last-child {
		@apply block lg:flex;
	}
</style>
