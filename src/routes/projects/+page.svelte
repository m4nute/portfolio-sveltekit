<script>
  import { MoveLeft } from "lucide-svelte"
  import ProjectCard from "../../components/homepage/projects/ProjectCard.svelte"
</script>

<a class="text-gray-400 inline-block hover:text-black dark:hover:text-white transition-all" href="/">
  <MoveLeft />
</a>
<br />
<h5 class="underline underline-offset-4 mb-3">Projects</h5>
<ol>
  <li class="flex flex-col gap-y-4">
    <ProjectCard
      project="This Portfolio"
      description="Personal Portfolio where I showcase my work, projects and skills. Also learned Svelte and testing along the way!"
      date="Aug 2023"
      link="https://manuelgudino.vercel.app/"
      badges={["SvelteKit", "Tailwind CSS", "Playwright", "Vitest"]}
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
    <ProjectCard
      project="PedaStore"
      description="An e-commerce website developed using Next.js, TypeScript, TailwindCSS, and NextAuth, with an integrated authentication system that allows registration using Google (OAuth 2.0) and regular credentials. This project is not finished and will be updated soon."
      date="Feb 2023"
      link="https://pedastore.vercel.app/"
      badges={["Next.js", "Tailwind CSS", "Supabase", "Zustand", "React Query"]}
      repo="https://github.com/m4nute/next-ecommerce"
    />
    <ProjectCard
      project="TopJobs"
      description="TopJobs is a job search website that provides daily job offers from the UK to all its users. The platform contains over 650 job listings from hundreds of companies, and it is updated daily with new opportunities, thanks to the public API of DevitJobsUK."
      date="Nov 2022"
      link="https://topjobs.netlify.app/"
      badges={["Next.js", "Tailwind CSS", "Supabase", "Zustand", "React Query"]}
    />
  </li>
</ol>
