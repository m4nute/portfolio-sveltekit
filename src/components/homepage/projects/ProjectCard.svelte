<script lang="ts">
  import { Badge } from "$lib/shadcn/ui/badge"
  import { Github } from "lucide-svelte"

  export let project: string
  export let date: string
  export let badges: string[]
  export let link: string
  export let description: string
  export let repo: string | null = null
</script>

<article class="flex flex-col sm:flex-row gap-2 sm:gap-6 mb-4">
  <section class="flex flex-row sm:flex-col justify-between py-1 sm:py-4">
    <div class="text-gray-800 dark:text-gray-200 text-sm w-24">{date}</div>
    {#if repo}
      <a
        class="flex w-fit hover:text-black dark:hover:text-white transition-all text-sm text-gray-600 dark:text-gray-300 gap-1"
        target="_blank"
        href={repo}><Github size={22} strokeWidth={1.6} /> <span>Repo</span></a
      >
    {/if}
  </section>
  <a
    target="_blank"
    href={link}
    class="flex-1 w-full hover:bg-[#eee] dark:hover:bg-[#112] cursor-pointer sm:p-4 rounded-lg transition-all duration-150"
  >
    <h6 class="font-bold text-lg">{project}</h6>
    <p class="text-sm text-gray-700 dark:text-gray-300 mt-1 mb-3">{description}</p>
    <ol class="gap-2 flex mt-3 flex-wrap">
      {#each badges as badge}
        <Badge>{badge}</Badge>
      {/each}
    </ol>
  </a>
</article>
