<script>
	import { Icon } from 'svelte-awesome';
	import { github, instagram, linkedinSquare, envelope } from 'svelte-awesome/icons';
	import Socials from './socials.svelte';
	import pfp from '$lib/imgs/pfp.webp?enhanced';

	const year = new Date().getFullYear();
</script>

<aside class="dark:text-white min-w-56 w-fit mt-8 left-32 pt-2 hidden md:block">
	<enhanced:img
		src={pfp}
		alt="Riley Smith looking at the aurora borealis"
		class="rounded-full w-24 h-24"
	/>
	<h1 class="text-2xl font-bold title">Riley Smith</h1>
	<p class="text-md text-gray-500 italic">Software Developer</p>
	<ul class="gap-y-2 mt-2 flex flex-col w-full">
		<li class="hover:underline">
			<a href="/">About</a>
		</li>
		<li class="hover:underline">
			<a href="/blog">Blog</a>
		</li>
		<li class="hover:underline">
			<a href="https://resume.rileyy.dev">Resume</a>
		</li>
		<li class="hidden hover:underline">
			<a href="/photography">Photography</a>
		</li>
	</ul>
	<!-- socials -->
	<Socials scale={1.5} />
	<footer class="mt-1">
		<a class="text-xs text-gray-500" href="https://github.com/rileyallyn/website">Source</a>
		<p class="text-xs text-gray-500">© 2024-{year} Riley Smith</p>
	</footer>
</aside>
