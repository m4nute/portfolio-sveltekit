<script lang="ts">
	import NavButton from './NavButton.svelte';
	import { FileText, Mail, Github, Linkedin } from 'lucide-svelte';
	import ThemeToggle from './ThemeToggle.svelte';
	let y: number;
</script>

<nav
	class="sticky top-2 rounded-xl bg-[#292929]/50 px-4 text-xl py-2 backdrop-blur-md flex justify-between"
>
	<section class="flex gap-3">
		<NavButton text={'Linkedin'}><Linkedin strokeWidth={1.6} size={22} /></NavButton>
		<NavButton text={'Github'}><Github strokeWidth={1.6} size={22} /></NavButton>
		<NavButton text={'Mail'}><Mail strokeWidth={1.6} size={22} /></NavButton>
		<NavButton text={'CV'}><FileText strokeWidth={1.6} size={22} /></NavButton>
	</section>
	<ThemeToggle />
</nav>

<svelte:window bind:scrollY={y} />
