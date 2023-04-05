<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div>
	<!-- Background -->
	<div class="relative overflow-hidden bg-orange-700 pb-16">
		<div
			aria-hidden="true"
			class="inset-y-0 absolute inset-x-0 left-1/2 w-full -translate-x-1/2 transform overflow-hidden lg:inset-y-0">
			<div class="absolute inset-0 flex">
				<div class="h-full w-full bg-gradient-to-r from-cyan-500 to-cyan-800" />
			</div>
		</div>
		<header class="relative py-10">
			<div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8" />
		</header>
	</div>

	<div class="relative -mt-12">
		<div class="mx-auto max-w-6xl px-4 pb-6 sm:px-6 lg:px-8 lg:pb-16">
			<!-- Question Input -->
			<div class="overflow-hidden rounded-lg bg-white shadow">
				<div
					class="divide-y divide-gray-200 lg:grid lg:grid-cols-12 lg:divide-x lg:divide-y-0">
					<form class="divide-y divide-gray-200 lg:col-span-12" action="#" method="POST">
						<div class="px-4 py-4">
							<!-- Question Input -->
							<div class="flex items-center justify-between lg:grid grid-cols-12">
								<div class="relative md:w-9/12 col-span-10">
									<input
										type="text"
										name="hs-search-box-with-loading-1"
										class="py-3 lg:px-4 block w-full border-none focus:outline-none font-light rounded-md text-base lg:text-2xl"
										placeholder="What is your question?" />
									<!-- Loading state TODO:Remove hidden class-->
									<div
										class="absolute inset-y-0 left-0 flex items-center pointer-events-none pl-4 hidden">
										<div
											class="animate-spin inline-block w-4 h-4 border-[3px] border-current border-t-transparent text-blue-600 rounded-full"
											role="status"
											aria-label="loading">
											<span class="sr-only">Loading...</span>
										</div>
									</div>
								</div>

								<div class="col-span-2 flex justify-end">
									<button
										type="button"
										class="py-2 lg:py-3 px-4 inline-flex justify-center items-center gap-2 rounded-md border border-transparent font-semibold bg-cyan-600 text-white">
										Ask <span class="hidden sm:block">a question</span>
									</button>
								</div>
							</div>
						</div>
					</form>
				</div>
			</div>

			<!-- Answers -->
			<div class="flex flex-col space-y-4 mt-12">
				<!-- Single Answers Card -->
				<div class="bg-white px-4 py-5 sm:px-6 rounded-lg shadow max-w-2xl">
					<article class="group relative flex flex-col items-start px-4 mt-6">
						<!-- Questions -->
						<blockquote class="relative">
							<svg
								class="absolute top-0 left-4 transform -translate-x-6 -translate-y-8 h-16 w-16 text-gray-100 dark:text-gray-700"
								width="16"
								height="16"
								viewBox="0 0 16 16"
								fill="none"
								xmlns="http://www.w3.org/2000/svg"
								aria-hidden="true">
								<path
									d="M7.39762 10.3C7.39762 11.0733 7.14888 11.7 6.6514 12.18C6.15392 12.6333 5.52552 12.86 4.76621 12.86C3.84979 12.86 3.09047 12.5533 2.48825 11.94C1.91222 11.3266 1.62421 10.4467 1.62421 9.29999C1.62421 8.07332 1.96459 6.87332 2.64535 5.69999C3.35231 4.49999 4.33418 3.55332 5.59098 2.85999L6.4943 4.25999C5.81354 4.73999 5.26369 5.27332 4.84476 5.85999C4.45201 6.44666 4.19017 7.12666 4.05926 7.89999C4.29491 7.79332 4.56983 7.73999 4.88403 7.73999C5.61716 7.73999 6.21938 7.97999 6.69067 8.45999C7.16197 8.93999 7.39762 9.55333 7.39762 10.3ZM14.6242 10.3C14.6242 11.0733 14.3755 11.7 13.878 12.18C13.3805 12.6333 12.7521 12.86 11.9928 12.86C11.0764 12.86 10.3171 12.5533 9.71484 11.94C9.13881 11.3266 8.85079 10.4467 8.85079 9.29999C8.85079 8.07332 9.19117 6.87332 9.87194 5.69999C10.5789 4.49999 11.5608 3.55332 12.8176 2.85999L13.7209 4.25999C13.0401 4.73999 12.4903 5.27332 12.0713 5.85999C11.6786 6.44666 11.4168 7.12666 11.2858 7.89999C11.5215 7.79332 11.7964 7.73999 12.1106 7.73999C12.8437 7.73999 13.446 7.97999 13.9173 8.45999C14.3886 8.93999 14.6242 9.55333 14.6242 10.3Z"
									fill="currentColor" />
							</svg>

							<div class="relative z-10">
								<p class="text-gray-800 sm:text-xl dark:text-white">
									<em> Was genau sind Strive Days? </em>
								</p>
							</div>
						</blockquote>

						<!-- Answer -->
						<div class="">
							<p class="relative z-10 mt-2 text-base text-zinc-500 font-light">
								Strive Days sind Meetings die stattfinden bei denen Themen
								besprochen werden die sich nicht für online Meetings eignen. Bisher
								in Nürnberg, Würzburg und Berlin. Immer auch mit etwas Spaß dabei.
							</p>
						</div>

						<div
							aria-hidden="true"
							class="relative z-10 mt-4 flex items-center text-sm font-light text-gray-300">
							Frage vom 12. Januar, 5:35 am
						</div>
					</article>
				</div>
			</div>

			<!-- CTA -->
			<div class="bg-cyan-600 rounded-lg mt-24">
				<div
					class="mx-auto max-w-7xl px-6 py-24 sm:py-32 lg:flex lg:items-center lg:justify-between lg:px-8">
					<h2 class="text-3xl font-bold tracking-tight text-white sm:text-4xl">
						Bereit AI zu wagen?<br />Buche einen Video-Call mit uns.
					</h2>
					<div
						class="mt-10 flex flex-col sm:flex-row items-center gap-x-6 lg:mt-0 lg:flex-shrink-0">
						<a
							href="https://www.bit.ly/3XBY2b4"
							target="_blank"
							class="rounded-md bg-white px-3.5 py-3.5 text-base font-semibold text-gray-800 shadow-sm">
							Jetzt Call buchen (30min)</a>
						<a
							href="https://www.strivestudio.de"
							target="_blank"
							class="mt-4 sm:mt-0 text-sm font-semibold leading-6 text-white">
							Strive Studio <span aria-hidden="true">→</span></a>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
