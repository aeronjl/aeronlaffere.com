<script>
	import '../app.css';
	import { fly } from 'svelte/transition';
</script>

<div class="flex max-h-screen min-h-screen items-center justify-center">
	<div
		class="md:grid flex flex-col max-h-[calc(100vh-2rem)] min-h-[calc(100vh-2rem)] min-w-[calc(100vw-2rem)] max-w-[calc(100vw-2rem)] grid-cols-9 gap-x-12 overflow-clip rounded border p-6 font-mono"
	>
		<div class="col-span-3 lg:mb-0 mb-12">
			<div class="flex flex-col gap-y-6">
				<a href="/" class="font-mono text-xs hover:underline">aeronlaffere.com</a>
				<div>
					<p class="text-2xl font-bold">Aeron Laffere</p>
					<p class="font-mono text-gray-500">Neuroscientist, Software Engineer</p>
				</div>
				<p class="text-sm">
					My main areas of research interest include <span class="font-bold"
						>psychiatric diagnosis</span
					>, <span class="font-bold">digital therapeutics</span>, and
					<span class="font-bold">defence applications</span> of cognitive science.
				</p>
				<hr />
				<div class="flex flex-row items-center gap-4">
					<a
						href="https://github.com/aeronjl"
						class=""
						target="_blank"
						rel="noopener noreferrer"
					>
						<svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 48 48">
							<path
								fill="none"
								stroke="currentColor"
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M24 2.5a21.5 21.5 0 0 0-6.8 41.9c1.08.2 1.47-.46 1.47-1v-3.65c-6 1.3-7.24-2.88-7.24-2.88A5.7 5.7 0 0 0 9 33.68c-1.95-1.33.15-1.31.15-1.31a4.52 4.52 0 0 1 3.29 2.22c1.92 3.29 5 2.34 6.26 1.79a4.6 4.6 0 0 1 1.37-2.88c-4.78-.54-9.8-2.38-9.8-10.62a8.3 8.3 0 0 1 2.22-5.77a7.68 7.68 0 0 1 .21-5.69s1.8-.58 5.91 2.2a20.46 20.46 0 0 1 10.76 0c4.11-2.78 5.91-2.2 5.91-2.2a7.74 7.74 0 0 1 .21 5.69a8.28 8.28 0 0 1 2.21 5.77c0 8.26-5 10.07-9.81 10.61a5.12 5.12 0 0 1 1.46 4v5.9c0 .71.39 1.24 1.48 1A21.5 21.5 0 0 0 24 2.5"
							/>
						</svg>
					</a>
					<a
						href="https://www.linkedin.com/in/aeronlaffere/"
						class=""
						target="_blank"
						rel="noopener noreferrer"
					>
						<svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 48 48">
							<path fill="currentColor" d="M25.388 22.34v-.056l-.037.057z" />
							<circle cx="15.64" cy="13.463" r=".75" fill="currentColor" />
							<path
								fill="none"
								stroke="currentColor"
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M15.64 16.93v14.982m17.47 0v-9.608a5.823 5.823 0 0 0-5.823-5.824h0a5.823 5.823 0 0 0-5.824 5.824v9.608m0-9.608V16.93"
							/>
							<path
								fill="none"
								stroke="currentColor"
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M38.5 5.5h-29a4 4 0 0 0-4 4v29a4 4 0 0 0 4 4h29a4 4 0 0 0 4-4v-29a4 4 0 0 0-4-4"
							/>
						</svg></a
					>
				</div>
			</div>
		</div>
		<div class="col-span-6 max-h-full overflow-y-scroll text-sm">
			<div class="flex h-full flex-col overflow-y-scroll">
				<div class="mb-4 flex flex-row gap-2">
					<a href="/" class="text-blue-600 underline">Blog</a>
					<a href="/bookmarks" class="text-blue-600 underline">Bookmarks</a>
					<a href="/projects" class="text-blue-600 underline">Projects</a>
				</div>
				<div class="flex-1 overflow-y-scroll">
					<slot></slot>
				</div>
			</div>
		</div>
	</div>
</div>

<style></style>
