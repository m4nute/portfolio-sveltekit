<script>
  import "../app.postcss"
  import Navbar from "../components/navbar/Navbar.svelte"
</script>

<main class="bg-white text-black dark:bg-[#1c1c1c] min-h-screen dark:text-white">
  <div class="max-w-2xl mx-auto">
    <Navbar />
    <div class="px-3 pt-8">
      <slot />
    </div>
  </div>
</main>
