<script lang="ts">
  export let y: number
  import { Moon, Sun } from "lucide-svelte"
  let isDark = false
  if (typeof localStorage !== "undefined") {
    if (localStorage.theme === "dark" || (!("theme" in localStorage) && window.matchMedia("(prefers-color-scheme: dark)").matches)) {
      isDark = true
    }
  }
  function toggleDarkMode() {
    if (isDark) {
      document.documentElement.classList.remove("dark")
      localStorage.theme = "light"
      isDark = false
    } else {
      document.documentElement.classList.add("dark")
      localStorage.theme = "dark"
      isDark = true
    }
  }
</script>

<button
  on:click={toggleDarkMode}
  class="p-2 hover:bg-yellow-500 {y > 70
    ? 'bg-[#e1e1e1] dark:bg-[#393939] dark:hover:bg-yellow-500 dark:hover:bg-opacity-30'
    : 'bg-transparent'} rounded-lg hover:bg-opacity-50 duration-150 transition-all overflow-hidden h-[38px]"
>
  {#if !isDark}
    <Moon strokeWidth={1.6} size={22} />
  {:else}
    <Sun strokeWidth={1.6} size={22} />
  {/if}
</button>
