<script lang="ts">
  import NavButton from "./NavButton.svelte"
  import { FileText, Mail, Github, Linkedin } from "lucide-svelte"
  import ThemeToggle from "./ThemeToggle.svelte"
  let y: number
</script>

<nav
  class="sticky top-2 px-4 text-xl mx-3 py-2 backdrop-blur-md border-b border-gray-300 dark:border-gray-600 border-opacity-50 transition-all
  flex justify-between {y > 70 ? 'bg-[#ededed] dark:bg-[#292929]/70 rounded-xl' : 'bg-transparent'}"
>
  <section class="flex gap-3">
    <NavButton link="https://www.linkedin.com/in/manuelgudino/" {y} text={"Linkedin"}><Linkedin strokeWidth={1.6} size={22} /></NavButton>
    <NavButton link="https://github.com/m4nute" {y} text={"Github"}><Github strokeWidth={1.6} size={22} /></NavButton>
    <NavButton link="mailto:mgudinocontacto@gmail.com?" {y} text={"Mail"}><Mail strokeWidth={1.6} size={22} /></NavButton>
    <NavButton link="/cv" {y} text={"CV"}><FileText strokeWidth={1.6} size={22} /></NavButton>
  </section>
  <ThemeToggle {y} />
</nav>

<svelte:window bind:scrollY={y} />
