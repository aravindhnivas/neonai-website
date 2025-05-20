<script lang="ts">
	const team = [
		{
			name: 'John Doe',
			role: 'CEO & Founder',
			image: 'https://picsum.photos/id/1/150',
			bio: 'Visionary leader with 15+ years of experience in AI and machine learning.'
		},
		{
			name: 'Jane Smith',
			role: 'CTO',
			image: 'https://picsum.photos/id/2/150',
			bio: 'Expert in deep learning and neural networks with multiple research papers published.'
		},
		{
			name: 'Mike Johnson',
			role: 'Lead AI Engineer',
			image: 'https://picsum.photos/id/3/150',
			bio: 'Specialist in natural language processing and computer vision.'
		}
	];
</script>

<div class="bg-white">
	<!-- Mission Section -->
	<div class="mx-auto max-w-7xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
		<div class="text-center">
			<h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl">
				Our Mission
			</h1>
			<p class="mx-auto mt-6 max-w-2xl text-xl text-gray-500">
				At NeonAI, we're dedicated to advancing artificial intelligence technology to solve
				real-world problems and create a better future for all.
			</p>
		</div>
	</div>

	<!-- Goals Section -->
	<div class="bg-gray-50">
		<div class="mx-auto max-w-7xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
			<div class="lg:text-center">
				<h2 class="text-base font-semibold tracking-wide text-indigo-600 uppercase">Goals</h2>
				<p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
					What We Strive For
				</p>
			</div>

			<div class="mt-10">
				<div class="space-y-10 md:grid md:grid-cols-2 md:space-y-0 md:gap-x-8 md:gap-y-10">
					<div class="relative">
						<div
							class="absolute flex h-12 w-12 items-center justify-center rounded-md bg-indigo-500 text-white"
						>
							<span class="text-2xl">🎯</span>
						</div>
						<div class="ml-16">
							<h3 class="text-lg leading-6 font-medium text-gray-900">Innovation</h3>
							<p class="mt-2 text-base text-gray-500">
								Continuously pushing the boundaries of what's possible with AI technology.
							</p>
						</div>
					</div>

					<div class="relative">
						<div
							class="absolute flex h-12 w-12 items-center justify-center rounded-md bg-indigo-500 text-white"
						>
							<span class="text-2xl">🤝</span>
						</div>
						<div class="ml-16">
							<h3 class="text-lg leading-6 font-medium text-gray-900">Collaboration</h3>
							<p class="mt-2 text-base text-gray-500">
								Working with partners and clients to create impactful AI solutions.
							</p>
						</div>
					</div>

					<div class="relative">
						<div
							class="absolute flex h-12 w-12 items-center justify-center rounded-md bg-indigo-500 text-white"
						>
							<span class="text-2xl">🌍</span>
						</div>
						<div class="ml-16">
							<h3 class="text-lg leading-6 font-medium text-gray-900">Impact</h3>
							<p class="mt-2 text-base text-gray-500">
								Making a positive difference in the world through AI technology.
							</p>
						</div>
					</div>

					<div class="relative">
						<div
							class="absolute flex h-12 w-12 items-center justify-center rounded-md bg-indigo-500 text-white"
						>
							<span class="text-2xl">📈</span>
						</div>
						<div class="ml-16">
							<h3 class="text-lg leading-6 font-medium text-gray-900">Growth</h3>
							<p class="mt-2 text-base text-gray-500">
								Expanding our capabilities and reach to serve more clients worldwide.
							</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<!-- Team Section -->
	<div class="mx-auto max-w-7xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
		<div class="lg:text-center">
			<h2 class="text-base font-semibold tracking-wide text-indigo-600 uppercase">Team</h2>
			<p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
				Meet Our Leadership
			</p>
		</div>

		<div class="mt-10">
			<div class="space-y-10 md:grid md:grid-cols-3 md:space-y-0 md:gap-x-8 md:gap-y-10">
				{#each team as member}
					<div class="text-center">
						<img class="mx-auto h-40 w-40 rounded-full" src={member.image} alt={member.name} />
						<h3 class="mt-6 text-lg font-medium text-gray-900">{member.name}</h3>
						<p class="text-sm text-indigo-600">{member.role}</p>
						<p class="mt-2 text-base text-gray-500">{member.bio}</p>
					</div>
				{/each}
			</div>
		</div>
	</div>
</div>
