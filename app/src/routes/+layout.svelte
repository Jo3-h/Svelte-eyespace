<!-- src/routes/+layout.svelte -->

<script lang="ts">
	import Navbar from '$lib/components/Navbar.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import '../app.css';

	let { children } = $props();
</script>
<div class="min-h-screen flex flex-col">
	<Navbar />
	<div class="flex-1 relative overflow-hidden">
		<video
		autoplay
		muted
		loop
		playsinline
		class="absolute top-0 left-0 w-full h-full object-cover z-[-1]"
		>
		<source src='/videos/bg-video.mp4' type="video/mp4" />
		Your Browser does not support the video tag.
	</video>
		{@render children()}
	</div>
	
	<Footer />
</div>


