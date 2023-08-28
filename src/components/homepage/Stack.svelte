<script lang="ts">
  let front: string[] = ["React", "Next.js", "TypeScript", "Tailwind CSS", "Shopify & Liquid", "SvelteKit"]
  let back: string[] = ["PostgreSQL", "MySQL", "Supabase", "Redis", "Node & Express.js", "Prisma ORM"]
  let test: string[] = ["Vitest", "Testing Library", "Playwright"]
</script>

<h5 class="underline underline-offset-4 mb-3">Skills</h5>
<ul class="flex flex-col gap-6">
  <li class="text-sm tracking-widest flex flex-col gap-y-2 sm:flex-row text-gray-800 dark:text-gray-200">
    <h6 class="w-32">• Front End:</h6>
    <div class="flex gap-x-2 gap-y-2 flex-wrap">
      {#each front as skill} <span class="px-2 py-1 bg-opacity-20 text-xs border rounded-2xl">{skill}</span> {/each}
    </div>
  </li>
  <li class="text-sm tracking-widest flex flex-col gap-y-2 sm:flex-row text-gray-800 dark:text-gray-200">
    <h6 class="w-32">• Back End:</h6>
    <div class="flex gap-x-2 gap-y-2 flex-wrap">
      {#each back as skill} <span class="px-2 py-1 bg-opacity-20 text-xs border rounded-2xl">{skill}</span> {/each}
    </div>
  </li>
  <li class="text-sm tracking-widest flex flex-col gap-y-2 sm:flex-row text-gray-800 dark:text-gray-200">
    <h6 class="w-28">• Testing:</h6>
    <div class="flex gap-x-2 gap-y-2 flex-wrap">
      {#each test as skill} <span class="px-2 py-1 bg-opacity-20 text-xs border rounded-2xl">{skill}</span> {/each}
    </div>
  </li>
</ul>
