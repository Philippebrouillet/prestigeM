<script>
	export let logo, agencyName;
</script>

<footer class="bg-primary py-8 px-6 lg:px-20 text-white">
	<div class="max-w-7xl mx-auto text-center">
		<!-- Logo -->
		<div class="mb-6">
			<img src={logo} alt={agencyName} class="mx-auto h-16 rounded-full" />
		</div>

		<!-- Agency Name -->
		<h2 class="text-2xl font-semibold mb-6 playfair">{agencyName}</h2>

		<!-- Navigation Links -->
		<nav class="mb-6">
			<ul class="flex flex-col sm:flex-row justify-center gap-2 sm:gap-6">
				<li><a href="#Solutions" class="navlink hover:text-tertiary">Solutions</a></li>
				<li><a href="#Results" class="navlink hover:text-tertiary">Results</a></li>
				<li><a href="#Services" class="navlink hover:text-tertiary">Services</a></li>
				<li><a href="#About" class="navlink hover:text-tertiary">About</a></li>
				<li><a href="#FAQ" class="navlink hover:text-tertiary">FAQ</a></li>
				<li><a href="#Contact" class="navlink hover:text-tertiary">Contact</a></li>
			</ul>
		</nav>

		<!-- Social Media Icons -->
		<div class="flex justify-center space-x-6 mb-6">
			<!-- Instagram Icon -->
			<a
				href="https://www.instagram.com"
				class="text-primary hover:text-secondary bg-white rounded-full p-2.5"
				aria-label="Instagram"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="h-6 w-6"
					viewBox="0 0 24 24"
				>
					<path
						d="M12 2.163c3.204 0 3.584.012 4.85.07 1.366.062 2.633.312 3.608 1.287.975.975 1.225 2.242 1.287 3.608.058 1.266.07 1.646.07 4.85s-.012 3.584-.07 4.85c-.062 1.366-.312 2.633-1.287 3.608-.975.975-2.242 1.225-3.608 1.287-1.266.058-1.646.07-4.85.07s-3.584-.012-4.85-.07c-1.366-.062-2.633-.312-3.608-1.287-.975-.975-1.225-2.242-1.287-3.608-.058-1.266-.07-1.646-.07-4.85s.012-3.584.07-4.85c.062-1.366.312-2.633 1.287-3.608.975-.975 2.242-1.225 3.608-1.287 1.266-.058 1.646-.07 4.85-.07zm0-2.163c-3.257 0-3.667.013-4.947.072-1.428.065-2.905.332-3.993 1.42-1.088 1.088-1.355 2.565-1.42 3.993-.059 1.281-.072 1.691-.072 4.947s.013 3.667.072 4.947c.065 1.428.332 2.905 1.42 3.993 1.088 1.088 2.565 1.355 3.993 1.42 1.281.059 1.691.072 4.947.072s3.667-.013 4.947-.072c1.428-.065 2.905-.332 3.993-1.42 1.088-1.088 1.355-2.565 1.42-3.993.059-1.281.072-1.691.072-4.947s-.013-3.667-.072-4.947c-.065-1.428-.332-2.905-1.42-3.993-1.088-1.088-2.565-1.355-3.993-1.42-1.281-.059-1.691-.072-4.947-.072z"
					/>
					<path
						d="M12 5.838a6.162 6.162 0 1 0 0 12.324 6.162 6.162 0 0 0 0-12.324zm0 10.162a3.999 3.999 0 1 1 0-7.998 3.999 3.999 0 0 1 0 7.998zm6.406-11.845a1.44 1.44 0 1 0 0 2.88 1.44 1.44 0 0 0 0-2.88z"
					/>
				</svg>
			</a>

			<!-- Facebook Icon -->
			<a
				href="https://www.facebook.com"
				class="text-primary hover:text-secondary bg-white rounded-full p-2.5"
				aria-label="Facebook"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="h-6 w-6"
					viewBox="0 0 24 24"
				>
					<path
						d="M22.676 0h-21.351c-.73 0-1.325.594-1.325 1.324v21.351c0 .73.594 1.325 1.325 1.325h11.492v-9.284h-3.124v-3.622h3.124v-2.671c0-3.1 1.893-4.788 4.656-4.788 1.325 0 2.462.099 2.795.142v3.241l-1.917.001c-1.504 0-1.795.716-1.795 1.764v2.311h3.587l-.467 3.622h-3.12v9.284h6.118c.73 0 1.325-.594 1.325-1.325v-21.35c0-.731-.595-1.325-1.325-1.325z"
					/>
				</svg>
			</a>

			<!-- WhatsApp Icon -->
			<a
				href="https://www.whatsapp.com"
				class="text-primary hover:text-secondary bg-white rounded-full p-2.5"
				aria-label="WhatsApp"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="currentColor"
					class="h-6 w-6"
					viewBox="0 0 24 24"
				>
					<path
						d="M16.555 13.412c-.265-.131-1.574-.777-1.819-.867-.242-.086-.419-.131-.595.132-.175.262-.681.867-.837 1.045-.155.175-.307.197-.573.065-.265-.131-1.118-.41-2.131-1.307-.788-.705-1.319-1.573-1.473-1.838-.155-.262-.017-.403.116-.532.119-.119.263-.309.394-.465.132-.154.175-.263.264-.438.087-.175.044-.328-.022-.465-.065-.131-.596-1.437-.816-1.976-.215-.517-.433-.446-.596-.456-.155-.013-.328-.016-.503-.016-.175 0-.46.065-.7.328-.242.262-.918.896-.918 2.185 0 1.287.94 2.531 1.07 2.705.131.175 1.855 2.841 4.501 3.985.629.272 1.118.434 1.501.559.63.2 1.2.175 1.654.106.504-.075 1.573-.643 1.794-1.268.22-.624.22-1.159.154-1.268-.065-.109-.242-.175-.507-.309zm-4.555 8.588c-1.333 0-2.632-.347-3.779-.1c0 0-.874 1.228-2.086 1.65c0 0 .407-1.288.497-1.512c-1.178-.922-2.034-2.114-2.486-3.507c-.494-1.522-.494-3.19 0-4.712c.47-1.429 1.361-2.649 2.486-3.506c.954-.769 2.062-1.269 3.227-1.48c1.174-.211 2.395-.061 3.479.44c1.084.5 2.035 1.267 2.798 2.235c.76.967 1.288 2.149 1.52 3.379c.23 1.23.132 2.49-.302 3.668c-.365 1.034-1.084 1.967-1.98 2.587c-.896.62-1.998.943-3.132.94z"
					/>
				</svg>
			</a>
		</div>

		<!-- Copyright Text -->
		<p class="text-sm mb-4">Copyright © 2024 • {agencyName}. All rights reserved.</p>

		<!-- Legal Links -->
		<div class="flex justify-center space-x-4 text-sm">
			<a href="#hero" class="hover:underline">Legal Notice</a>
			<span class="text-gray-400">|</span>
			<a href="#hero" class="hover:underline">Privacy Policy</a>
			<span class="text-gray-400">|</span>
			<a href="#hero" class="hover:underline">Cookie Policy</a>
		</div>
	</div>

	<!-- Bottom Bar -->
	<div class="bg-primary-dark py-2 mt-8 text-center text-sm">
		<p class="text-gray-800 font-semibold">
			Design, text, and development by <a href="#hero" class="text-white hover:underline">PB</a>
		</p>
	</div>
</footer>
