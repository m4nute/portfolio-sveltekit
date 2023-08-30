<script>
  import Contact from "../components/homepage/Contact.svelte"
  import Experience from "../components/homepage/experience/Experience.svelte"
  import Intro from "../components/homepage/Intro.svelte"
  import Projects from "../components/homepage/projects/Projects.svelte"
  import Stack from "../components/homepage/Stack.svelte"
</script>

<svelte:head>
  <title>Manuel Gudiño</title>
</svelte:head>

<div>
  <Intro />
  <br /><br />
  <Experience />
  <br /><br />
  <Projects />
  <br /><br />
  <Stack />
  <br /><br />
  <Contact />
</div>
