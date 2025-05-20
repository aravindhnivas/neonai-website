<script lang="ts">
	const projects = [
		{
			title: 'AI-Powered Analytics Platform',
			description:
				'A comprehensive analytics solution that leverages machine learning to provide actionable insights from complex data sets.',
			image: 'https://via.placeholder.com/600x400',
			technologies: ['Machine Learning', 'Python', 'TensorFlow', 'React'],
			link: '#'
		},
		{
			title: 'Natural Language Processing API',
			description:
				'Advanced NLP capabilities for text analysis, sentiment analysis, and language understanding.',
			image: 'https://via.placeholder.com/600x400',
			technologies: ['NLP', 'Python', 'FastAPI', 'Docker'],
			link: '#'
		},
		{
			title: 'Computer Vision System',
			description:
				'Real-time object detection and image recognition system for industrial applications.',
			image: 'https://via.placeholder.com/600x400',
			technologies: ['Computer Vision', 'PyTorch', 'OpenCV', 'C++'],
			link: '#'
		},
		{
			title: 'AI Chatbot Framework',
			description:
				'Customizable chatbot framework that can be trained for specific business domains.',
			image: 'https://via.placeholder.com/600x400',
			technologies: ['Deep Learning', 'Python', 'TensorFlow', 'Node.js'],
			link: '#'
		}
	];
</script>

<div class="bg-white">
	<div class="mx-auto max-w-7xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
		<div class="text-center">
			<h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl">
				Our Projects
			</h1>
			<p class="mx-auto mt-6 max-w-2xl text-xl text-gray-500">
				Explore our innovative AI solutions and cutting-edge projects that are transforming
				industries.
			</p>
		</div>

		<div class="mt-12 grid gap-8 md:grid-cols-2">
			{#each projects as project}
				<div class="overflow-hidden rounded-lg bg-white shadow">
					<div class="relative">
						<img class="h-48 w-full object-cover" src={project.image} alt={project.title} />
						<div
							class="absolute inset-0 flex items-center justify-center bg-indigo-600 opacity-0 transition-opacity duration-300 hover:opacity-75"
						>
							<a
								href={project.link}
								class="rounded-md border-2 border-white px-4 py-2 font-semibold text-white transition-colors duration-300 hover:bg-white hover:text-indigo-600"
							>
								Learn More
							</a>
						</div>
					</div>
					<div class="px-4 py-5 sm:p-6">
						<h3 class="text-lg font-medium text-gray-900">{project.title}</h3>
						<p class="mt-2 text-sm text-gray-500">{project.description}</p>
						<div class="mt-4 flex flex-wrap gap-2">
							{#each project.technologies as tech}
								<span
									class="inline-flex items-center rounded-full bg-indigo-100 px-2.5 py-0.5 text-xs font-medium text-indigo-800"
								>
									{tech}
								</span>
							{/each}
						</div>
					</div>
				</div>
			{/each}
		</div>

		<!-- Call to Action -->
		<div class="mt-16 text-center">
			<h2 class="text-2xl font-bold text-gray-900">Ready to Start Your Project?</h2>
			<p class="mt-4 text-lg text-gray-500">
				Let's discuss how we can help you achieve your goals with AI technology.
			</p>
			<div class="mt-8">
				<a
					href="/contact"
					class="inline-flex items-center rounded-md border border-transparent bg-indigo-600 px-6 py-3 text-base font-medium text-white hover:bg-indigo-700"
				>
					Contact Us
				</a>
			</div>
		</div>
	</div>
</div>
