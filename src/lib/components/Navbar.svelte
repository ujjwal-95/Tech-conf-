<script>
  import "bootstrap/dist/css/bootstrap.min.css";
  import { onMount } from "svelte";

  let collapse;

  onMount(async () => {
    const { Collapse } = await import("bootstrap");
    collapse = new Collapse(document.getElementById("navbarNav"), { toggle: false });
  });

  function toggleNavbar() {
    collapse.toggle();
  }

  function closeNavbar() {
    collapse.hide();
  }
</script>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="/">TechConf</a>

    <button 
      class="navbar-toggler" 
      type="button" 
      on:click={toggleNavbar}
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse justify-content-lg-end" id="navbarNav">
      <ul class="navbar-nav ms-lg-auto text-lg-center">
        <li class="nav-item">
          <a class="nav-link" href="/speakers" on:click={closeNavbar}>Speakers</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/schedule" on:click={closeNavbar}>Schedule</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/sponsors" on:click={closeNavbar}>Sponsors</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/about" on:click={closeNavbar}>About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/contact" on:click={closeNavbar}>Contact</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
