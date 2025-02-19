<script lang="ts">
	export const prerender = true
	import '../app.css';
	let { children } = $props();
</script>

<!-- Main Container -->
<div class="animate__animated animate__fadeIn animate__slow mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
	<!-- Inner Wrapper -->
	<div class="mx-auto max-w-5xl">
			{@render children()}
	</div>
</div>