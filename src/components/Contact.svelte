<script>
	import emailjs from 'emailjs-com';
	import { toast } from 'svelte-sonner';

	export let agencyName;

	emailjs.init('TcZbVBBUg-p6ppXEA');

	function handleSubmit(e) {
		e.preventDefault();
		toast.promise(emailjs.sendForm('mia', 'template_xu10eax', e.target), {
			loading: 'Loading...',
			success: 'Message sent successfully!',
			error: 'Error... :( Try again!'
		});
	}
</script>

<section
	id="Contact"
	class="bg-gradient-to-b from-primary via-secondary to-primary py-28 my-10 px-6 lg:px-20 text-white"
>
	<div class="max-w-4xl mx-auto">
		<h2 class="text-3xl lg:text-4xl font-semibold playfair text-center mb-10">
			Join {agencyName} and Boost Your OnlyFans & MYM Earnings
		</h2>
		<p class="lg:text-lg text-center mb-12">
			Send us your application and we will get back to you as soon as possible.
		</p>

		<form class="space-y-5" on:submit={handleSubmit}>
			<!-- General Information -->
			<div class="space-y-6">
				<h3 class="text-lg font-semibold border-b-2 border-white pb-2">General Information</h3>
				<div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
					<input
						type="text"
						name="name"
						placeholder="Your Name *"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
						required
					/>
					<input
						type="text"
						name="username"
						placeholder="Your Username"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
					<input
						type="email"
						name="email"
						placeholder="Email Address *"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
						required
					/>
					<input
						type="text"
						name="phone"
						placeholder="Phone (WhatsApp)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
				</div>
			</div>

			<!-- Social Media -->
			<div class="space-y-6">
				<h3 class="text-lg font-semibold border-b-2 border-white pb-2">Your Social Media</h3>
				<div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
					<input
						type="text"
						name="instagram"
						placeholder="Instagram (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
					<input
						type="text"
						name="tiktok"
						placeholder="TikTok (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
					<input
						type="text"
						name="twitter"
						placeholder="Twitter (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
					<input
						type="text"
						name="snapchat"
						placeholder="Snapchat (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
				</div>
			</div>

			<!-- Platforms -->
			<div class="space-y-6">
				<h3 class="text-lg font-semibold border-b-2 border-white pb-2">
					Your OnlyFans & MYM Platforms
				</h3>
				<div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
					<input
						type="text"
						name="onlyfans"
						placeholder="OnlyFans (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
					<input
						type="text"
						name="mym"
						placeholder="MYM (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg focus:outline-none focus:ring-4 focus:ring-secondary transition"
					/>
				</div>
			</div>

			<!-- Additional Information -->
			<div class="space-y-6">
				<h3 class="text-lg font-semibold border-b-2 border-white pb-2">Additional Information</h3>
				<div class="space-y-6">
					<div>
						<label for="earnings" class="block mb-2 font-medium"
							>Current Monthly Earnings from these Platforms *</label
						>
						<select
							name="earnings"
							class="bg-tertiary text-gray-700 p-3 rounded-lg w-full focus:outline-none focus:ring-4 focus:ring-secondary transition"
							required
						>
							<option value="less than $500">Less than $500</option>
							<option value="$500 - $1000">$500 - $1000</option>
							<option value="$1000 - $5000">$1000 - $5000</option>
							<option value="more than $5000">More than $5000</option>
						</select>
					</div>
					<div>
						<label for="timeDedication" class="block mb-2 font-medium"
							>Time Dedication to OnlyFans/MYM *</label
						>
						<select
							name="timeDedication"
							class="bg-tertiary text-gray-700 p-3 rounded-lg w-full focus:outline-none focus:ring-4 focus:ring-secondary transition"
							required
						>
							<option value="part-time">Part-time</option>
							<option value="full-time">Full-time</option>
							<option value="as a hobby">As a hobby</option>
						</select>
					</div>
					<textarea
						name="message"
						placeholder="Your message, additional information, motivation... (optional)"
						class="bg-tertiary text-gray-700 p-3 rounded-lg w-full focus:outline-none focus:ring-4 focus:ring-secondary transition"
					></textarea>
				</div>
			</div>

			<!-- Submit Button -->
			<div class="flex justify-center">
				<button
					type="submit"
					class="linkButtonPrimary w-full sm:w-1/3 py-4 text-lg font-semibold tracking-wide bg-secondary hover:bg-secondary/80 text-white"
				>
					Send Application
				</button>
			</div>
		</form>
	</div>
</section>
