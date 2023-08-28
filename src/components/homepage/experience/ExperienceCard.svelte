<script lang="ts">
  import { Badge } from "$lib/shadcn/ui/badge"
  export let badges: string[]
  export let project: string
  export let role: string
  export let link: string
  export let description: string
  export let duration: string
  export let achievements: string[]
</script>

<article class="flex gap-2 sm:gap-8 flex-col sm:flex-row">
  <div class="text-gray-800 dark:text-gray-200 text-sm pt-4 w-32">{duration}</div>
  <a target="_blank" href={link} class="flex-1 hover:bg-[#eee] dark:hover:bg-[#112] cursor-pointer p-0 sm:p-4 rounded-lg transition-all duration-150">
    <h6 class="font-bold text-lg">{project}</h6>
    <span>{role}</span>
    <p class="text-sm text-gray-700 dark:text-gray-300 mb-3">{description}</p>
    <ul class="gap-1 flex flex-col">
      {#each achievements as achievement}
        <li class="text-xs text-gray-700 dark:text-gray-300"><strong>•</strong> {achievement}</li>
      {/each}
    </ul>
    <ol class="gap-2 flex mt-3 flex-wrap">
      {#each badges as badge}
        <Badge>{badge}</Badge>
      {/each}
    </ol>
  </a>
</article>
