<script>
	import { Moon, Sun } from 'lucide-svelte';
	import { fade, fly } from 'svelte/transition';
	let isDark = false;
	if (typeof localStorage !== 'undefined') {
		if (
			localStorage.theme === 'dark' ||
			(!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)
		) {
			isDark = true;
		}
	}
	function toggleDarkMode() {
		if (isDark) {
			document.documentElement.classList.remove('dark');
			localStorage.theme = 'light';
			isDark = false;
		} else {
			document.documentElement.classList.add('dark');
			localStorage.theme = 'dark';
			isDark = true;
		}
	}
</script>

<button
	on:click={toggleDarkMode}
	class="p-2 bg-[#393939] rounded-lg hover:bg-yellow-500 hover:bg-opacity-20 duration-150 transition-all overflow-hidden h-[38px]"
>
	{#if isDark}
		<Moon strokeWidth={1.6} size={22} />
	{:else}
		<Sun strokeWidth={1.6} size={22} color={'#ddd'} />
	{/if}
</button>
