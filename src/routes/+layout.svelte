<script>
  import "bootstrap/dist/css/bootstrap.min.css";
  import Navbar from "../lib/components/Navbar.svelte";
  import Footer from "../lib/components/Footer.svelte";
</script>

<div class="d-flex flex-column min-vh-100">
  <Navbar />
  
  <main class="flex-grow-1">
    <slot />
  </main>

  <Footer />
</div>
