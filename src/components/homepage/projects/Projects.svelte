<script>
  import ProjectCard from "./ProjectCard.svelte"
</script>

<h5 class="underline underline-offset-4 mb-3">Projects</h5>
<ol>
  <li class="flex flex-col gap-y-4">
    <ProjectCard
      project="This Portfolio"
      description="Personal Portfolio where I showcase my work, projects and skills."
      date="Aug 2023"
      link="https://mgud.vercel.app/"
      badges={["SvelteKit", "Tailwind CSS", "TypeScript"]}
      repo="https://github.com/m4nute/portfolio-sveltekit"
    />
    <ProjectCard
      project="Personal Blog"
      description="Personal blog where I talk about the technologies I'm passionate about and share my experiences and knowledge about them."
      date="May 2023"
      link="https://manuelgudino-blog.vercel.app"
      badges={["Next.js", "Tailwind CSS", "ContentLayer"]}
      repo="https://github.com/m4nute/blog-next13-contentlayer"
    />
    <ProjectCard
      project="Realtime Chat App"
      description="Contains Google and credentials auth, private chat rooms, realtime messages and chat list ordered by last update."
      date="May 2023"
      link="https://m4nute-chat.vercel.app/"
      badges={["Next.js", "Tailwind CSS", "Supabase", "Zustand", "React Query"]}
      repo="https://github.com/m4nute/next-supa-chat"
    />
  </li>
</ol>
<br />
<div class="text-center">
  <a href="/projects" class="underline underline-offset-2 text-gray-700 hover:text-black dark:text-gray-300 dark:hover:text-white transition-all"
    >View All Projects</a
  >
</div>
