<script>
	import '../app.postcss';
	import './styles.css';
</script>

<!-- ========== HEADER ========== -->
<header
	class="flex flex-wrap sm:justify-start sm:flex-nowrap z-50 w-full bg-white border-b text-sm py-2.5 sm:py-4 dark:bg-slate-900 dark:border-gray-700">
	<nav
		class="max-w-7xl flex basis-full items-center w-full mx-auto px-4 sm:px-6 lg:px-8"
		aria-label="Global">
		<div class="mr-5 md:mr-8">
			<img
				src="https://uploads-ssl.webflow.com/63e5ff4d535a98822fc01b69/642b4942d4d87f5a2688df45_ibot.png"
				alt="Logo"
				width="80px" />
		</div>

		<div
			class="w-full flex items-center justify-end ml-auto sm:justify-between sm:gap-x-3 sm:order-3">
			<div class="sm:hidden">
				<button
					type="button"
					class="inline-flex flex-shrink-0 justify-center items-center gap-2 h-[2.375rem] w-[2.375rem] rounded-full font-medium bg-white text-gray-700 align-middle hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-gray-400 focus:ring-offset-2 focus:ring-offset-white transition-all text-xs dark:bg-gray-800 dark:hover:bg-slate-800 dark:text-gray-400 dark:hover:text-white dark:focus:ring-gray-700 dark:focus:ring-offset-gray-800">
					<svg
						class="w-3.5 h-3.5"
						xmlns="http://www.w3.org/2000/svg"
						width="16"
						height="16"
						fill="currentColor"
						viewBox="0 0 16 16">
						<path
							d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z" />
					</svg>
				</button>
			</div>

			<div class="hidden sm:block">
				<label for="icon" class="sr-only" />
			</div>

			<div class="flex flex-row items-center justify-end gap-2">
				<div
					class="hs-dropdown relative inline-flex"
					data-hs-dropdown-placement="bottom-right">
					<button
						id="hs-dropdown-with-header"
						type="button"
						class="hs-dropdown-toggle inline-flex flex-shrink-0 justify-center items-center gap-2 h-[2.375rem] w-[2.375rem] rounded-full font-medium bg-white text-gray-700 align-middle hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-gray-400 focus:ring-offset-2 focus:ring-offset-white transition-all text-xs dark:bg-gray-800 dark:hover:bg-slate-800 dark:text-gray-400 dark:hover:text-white dark:focus:ring-gray-700 dark:focus:ring-offset-gray-800">
						<img
							class="inline-block h-[2.375rem] w-[2.375rem] rounded-full ring-2 ring-white dark:ring-gray-800"
							src="https://uploads-ssl.webflow.com/63e5ff4d535a98822fc01b69/642b4a1ca2fa0304137b879e_ai3.png"
							alt="Avatar" />
					</button>
				</div>
			</div>
		</div>
	</nav>
</header>
<!-- ========== END HEADER ========== -->

<div class="app">
	<main>
		<slot />
	</main>
</div>
