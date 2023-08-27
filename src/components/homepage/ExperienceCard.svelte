<script lang="ts">
  import { Badge } from "$lib/shadcn/ui/badge"
  export let badges: string[]
  export let project: string
  export let role: string
  export let link: string
  export let description: string
  export let duration: string
</script>

<article class="flex gap-24">
  <div class="text-gray-800 dark:text-gray-200 text-sm pt-4 w-32">{duration}</div>
  <a target="_blank" href={link} class="flex-1 hover:bg-[#ddd] dark:hover:bg-[#112] cursor-pointer p-4 rounded-lg transition-all duration-150">
    <h6 class="font-bold">{project}</h6>
    <span class="text-sm">{role}</span>
    <p class="text-xs text-gray-700 dark:text-gray-300 mb-3">{description}</p>
    <ol class="gap-2 flex">
      {#each badges as badge}
        <Badge>{badge}</Badge>
      {/each}
    </ol>
  </a>
</article>
