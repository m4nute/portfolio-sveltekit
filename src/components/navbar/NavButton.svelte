<script lang="ts">
  import * as Tooltip from "$lib/shadcn/ui/tooltip"
  export let text: string
  export let y: number
  export let link: string
</script>

<Tooltip.Root openDelay={120}>
  <Tooltip.Trigger>
    <!-- bg-[#e1e1e1] dark:bg-[#393939] -->
    <button
      on:click={() => window.open(link, "_blank")}
      class="{y > 70 ? '' : 'bg-transparent'} p-2 rounded-lg hover:scale-105 duration-150 transition-transform"
    >
      <slot />
    </button>
  </Tooltip.Trigger>
  <Tooltip.Content class="bg-[#efefef] dark:bg-[#393939] font-bold border-gray-600 border-opacity-10">
    <h4 class="text-xs">{text}</h4>
  </Tooltip.Content>
</Tooltip.Root>
