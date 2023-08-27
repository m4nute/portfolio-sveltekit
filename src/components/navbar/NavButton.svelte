<script lang="ts">
  import * as Tooltip from "$lib/shadcn/ui/tooltip"
  export let text: string
</script>

<Tooltip.Root openDelay={120}>
  <Tooltip.Trigger>
    <button class="bg-[#393939] p-2 rounded-lg hover:scale-105 duration-150 transition-transform">
      <slot />
    </button>
  </Tooltip.Trigger>
  <Tooltip.Content class="bg-[#393939] font-bold border-gray-100 border-opacity-10">
    <h4 class="text-xs">{text}</h4>
  </Tooltip.Content>
</Tooltip.Root>
