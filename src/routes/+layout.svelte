<script lang="ts">
	import '../app.css';
</script>

<div class="flex min-h-screen flex-col">
	<header class="bg-white shadow-sm">
		<nav class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
			<div class="flex h-16 justify-between">
				<div class="flex">
					<div class="flex flex-shrink-0 items-center">
						<a href="/" class="text-2xl font-bold text-indigo-600">NeonAI</a>
					</div>
					<div class="hidden sm:ml-6 sm:flex sm:space-x-8">
						<a
							href="/"
							class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-medium text-gray-500 hover:border-gray-300 hover:text-gray-700"
						>
							Home
						</a>
						<a
							href="/about"
							class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-medium text-gray-500 hover:border-gray-300 hover:text-gray-700"
						>
							About
						</a>
						<a
							href="/projects"
							class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-medium text-gray-500 hover:border-gray-300 hover:text-gray-700"
						>
							Projects
						</a>
						<a
							href="/contact"
							class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-medium text-gray-500 hover:border-gray-300 hover:text-gray-700"
						>
							Contact
						</a>
					</div>
				</div>
			</div>
		</nav>
	</header>

	<main class="flex-grow">
		<slot />
	</main>

	<footer class="bg-gray-800 text-white">
		<div class="mx-auto max-w-7xl px-4 py-12 sm:px-6 lg:px-8">
			<div class="grid grid-cols-1 gap-8 md:grid-cols-3">
				<div>
					<h3 class="mb-4 text-lg font-semibold">NeonAI</h3>
					<p class="text-gray-300">Advancing artificial intelligence for a better future.</p>
				</div>
				<div>
					<h3 class="mb-4 text-lg font-semibold">Quick Links</h3>
					<ul class="space-y-2">
						<li><a href="/about" class="text-gray-300 hover:text-white">About Us</a></li>
						<li><a href="/projects" class="text-gray-300 hover:text-white">Projects</a></li>
						<li><a href="/contact" class="text-gray-300 hover:text-white">Contact</a></li>
					</ul>
				</div>
				<div>
					<h3 class="mb-4 text-lg font-semibold">Contact</h3>
					<p class="text-gray-300">Email: contact@neonai.com</p>
				</div>
			</div>
			<div class="mt-8 border-t border-gray-700 pt-8 text-center text-gray-300">
				<p>&copy; {new Date().getFullYear()} NeonAI. All rights reserved.</p>
			</div>
		</div>
	</footer>
</div>
