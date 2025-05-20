<script lang="ts">
	let formData = {
		name: '',
		email: '',
		company: '',
		message: ''
	};

	let isSubmitting = false;
	let submitSuccess = false;
	let submitError = false;

	async function handleSubmit() {
		isSubmitting = true;
		submitSuccess = false;
		submitError = false;

		try {
			// Here you would typically send the form data to your backend
			await new Promise((resolve) => setTimeout(resolve, 1000)); // Simulated API call
			submitSuccess = true;
			formData = { name: '', email: '', company: '', message: '' };
		} catch (error) {
			submitError = true;
		} finally {
			isSubmitting = false;
		}
	}
</script>

<div class="bg-white">
	<div class="mx-auto max-w-7xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
		<div class="text-center">
			<h1 class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl">
				Contact Us
			</h1>
			<p class="mx-auto mt-6 max-w-2xl text-xl text-gray-500">
				Get in touch with our team to discuss how we can help transform your business with AI.
			</p>
		</div>

		<div class="mt-16 grid grid-cols-1 gap-8 md:grid-cols-2">
			<!-- Contact Information -->
			<div class="rounded-lg bg-gray-50 p-8">
				<h2 class="mb-6 text-2xl font-bold text-gray-900">Get in Touch</h2>

				<div class="space-y-6">
					<div>
						<h3 class="text-lg font-medium text-gray-900">Address</h3>
						<p class="mt-2 text-gray-500">
							123 AI Street<br />
							Tech City, TC 12345<br />
							United States
						</p>
					</div>

					<div>
						<h3 class="text-lg font-medium text-gray-900">Email</h3>
						<p class="mt-2 text-gray-500">
							<a href="mailto:contact@neonai.com" class="text-indigo-600 hover:text-indigo-500">
								contact@neonai.com
							</a>
						</p>
					</div>

					<div>
						<h3 class="text-lg font-medium text-gray-900">Phone</h3>
						<p class="mt-2 text-gray-500">
							<a href="tel:+1-555-123-4567" class="text-indigo-600 hover:text-indigo-500">
								+1 (555) 123-4567
							</a>
						</p>
					</div>
				</div>
			</div>

			<!-- Contact Form -->
			<div class="rounded-lg bg-white p-8 shadow">
				<form on:submit|preventDefault={handleSubmit} class="space-y-6">
					<div>
						<label for="name" class="block text-sm font-medium text-gray-700">Name</label>
						<input
							type="text"
							id="name"
							bind:value={formData.name}
							required
							class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
						/>
					</div>

					<div>
						<label for="email" class="block text-sm font-medium text-gray-700">Email</label>
						<input
							type="email"
							id="email"
							bind:value={formData.email}
							required
							class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
						/>
					</div>

					<div>
						<label for="company" class="block text-sm font-medium text-gray-700">Company</label>
						<input
							type="text"
							id="company"
							bind:value={formData.company}
							class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
						/>
					</div>

					<div>
						<label for="message" class="block text-sm font-medium text-gray-700">Message</label>
						<textarea
							id="message"
							bind:value={formData.message}
							required
							rows="4"
							class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-500 focus:ring-indigo-500"
						></textarea>
					</div>

					<div>
						<button
							type="submit"
							disabled={isSubmitting}
							class="flex w-full justify-center rounded-md border border-transparent bg-indigo-600 px-4 py-2 text-sm font-medium text-white shadow-sm hover:bg-indigo-700 focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2 focus:outline-none disabled:opacity-50"
						>
							{isSubmitting ? 'Sending...' : 'Send Message'}
						</button>
					</div>

					{#if submitSuccess}
						<div class="rounded-md bg-green-50 p-4">
							<div class="flex">
								<div class="flex-shrink-0">
									<span class="text-green-400">✓</span>
								</div>
								<div class="ml-3">
									<p class="text-sm font-medium text-green-800">
										Thank you for your message! We'll get back to you soon.
									</p>
								</div>
							</div>
						</div>
					{/if}

					{#if submitError}
						<div class="rounded-md bg-red-50 p-4">
							<div class="flex">
								<div class="flex-shrink-0">
									<span class="text-red-400">✕</span>
								</div>
								<div class="ml-3">
									<p class="text-sm font-medium text-red-800">
										Sorry, there was an error sending your message. Please try again.
									</p>
								</div>
							</div>
						</div>
					{/if}
				</form>
			</div>
		</div>
	</div>
</div>
