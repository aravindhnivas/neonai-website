<script lang="ts">
	const features = [
		{
			title: 'AI Innovation',
			description:
				'Pushing the boundaries of artificial intelligence with cutting-edge research and development.',
			icon: '🚀'
		},
		{
			title: 'Custom Solutions',
			description:
				'Tailored AI solutions designed to meet your specific business needs and challenges.',
			icon: '⚡'
		},
		{
			title: 'Expert Team',
			description:
				'Our team of AI specialists brings years of experience in machine learning and deep learning.',
			icon: '👥'
		}
	];
</script>

<div class="bg-white">
	<!-- Hero Section -->
	<div class="relative bg-indigo-800">
		<div class="absolute inset-0">
			<div class="absolute inset-0 bg-indigo-800 mix-blend-multiply"></div>
		</div>
		<div class="relative mx-auto max-w-7xl px-4 py-24 sm:px-6 sm:py-32 lg:px-8">
			<h1 class="text-4xl font-extrabold tracking-tight text-white sm:text-5xl lg:text-6xl">
				Welcome to NeonAI
			</h1>
			<p class="mt-6 max-w-3xl text-xl text-indigo-100">
				Welcome to the Landing Page of the NEON Project, an initiative by Neurale Fisica. We are
				extremely delighted by your shown interest in our endeavour. Buckle up and get ready for a
				captivating journey through which we unveil our services, which not only make you more
				productive but also the greater development of the human society, more sustainable.
			</p>
			<div class="mt-10">
				<a
					href="/contact"
					class="inline-flex items-center rounded-md border border-transparent bg-white px-6 py-3 text-base font-medium text-indigo-700 hover:bg-indigo-50"
				>
					Get Started
				</a>
			</div>
		</div>
	</div>

	<!-- Features Section -->
	<div class="bg-white py-12">
		<div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
			<div class="lg:text-center">
				<h2 class="text-base font-semibold tracking-wide text-indigo-600 uppercase">Features</h2>
				<p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
					Why Choose NeonAI?
				</p>
			</div>

			<div class="mt-10">
				<div class="space-y-10 md:grid md:grid-cols-3 md:space-y-0 md:gap-x-8 md:gap-y-10">
					{#each features as feature}
						<div class="relative">
							<div
								class="absolute flex h-12 w-12 items-center justify-center rounded-md bg-indigo-500 text-white"
							>
								<span class="text-2xl">{feature.icon}</span>
							</div>
							<div class="ml-16">
								<h3 class="text-lg leading-6 font-medium text-gray-900">{feature.title}</h3>
								<p class="mt-2 text-base text-gray-500">{feature.description}</p>
							</div>
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>

	<!-- CTA Section -->
	<div class="bg-indigo-50">
		<div
			class="mx-auto max-w-7xl px-4 py-12 sm:px-6 lg:flex lg:items-center lg:justify-between lg:px-8 lg:py-16"
		>
			<h2 class="text-3xl font-extrabold tracking-tight text-gray-900 sm:text-4xl">
				<span class="block">Ready to get started?</span>
				<span class="block text-indigo-600">Contact us today.</span>
			</h2>
			<div class="mt-8 flex lg:mt-0 lg:flex-shrink-0">
				<div class="inline-flex rounded-md shadow">
					<a
						href="/contact"
						class="inline-flex items-center justify-center rounded-md border border-transparent bg-indigo-600 px-5 py-3 text-base font-medium text-white hover:bg-indigo-700"
					>
						Contact Us
					</a>
				</div>
			</div>
		</div>
	</div>
</div>
