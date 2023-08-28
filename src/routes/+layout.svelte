<script>
  import "../app.postcss"
  import Footer from "../components/Footer.svelte"
  import Navbar from "../components/navbar/Navbar.svelte"
</script>

<main class="bg-white text-black dark:bg-[#1c1c1c] min-h-screen dark:text-white">
  <div class="max-w-2xl mx-auto">
    <Navbar />
    <div class="px-4 pt-10 pb-6">
      <slot />
    </div>
    <Footer />
  </div>
</main>
