<script lang="ts">
	import { CircleArrowRight } from 'lucide-svelte';

	export let href: string = '/';
	export let size: number = 14;
</script>

<a {href}>
	<slot />
	<CircleArrowRight {size} />
</a>

<style>
	a {
    padding-block: 1rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
		font-size: 1.1rem;
		font-weight: 600;
		text-decoration: none;
		color: var(--primary);
	}
</style>
