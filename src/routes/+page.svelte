<script>
  export let speakers = [
    { name: "John Doe", title: "AI Researcher", image: "/expert1.jpg" },
    { name: "Jane Smith", title: "Cybersecurity Expert", image: "/expert2.jpg" },
    { name: "Alice Johnson", title: "Blockchain Developer", image: "/expert3.png" }
  ];
</script>

<section class="hero text-center text-white bg-dark py-5">
  <div class="container">
    <h1 class="display-4">Welcome to TechConf 2025</h1>
    <p class="lead">Join the future of technology and innovation.</p>
    <a href="/" class="btn btn-primary btn-lg">Register Now</a>
  </div>
</section>

<!-- Featured Speakers Section -->
<section class="featured-speakers py-5 bg-light">
  <div class="container">
    <h2 class="text-center mb-4">Featured Speakers</h2>
    <div class="row">
      {#each speakers as speaker}
        <div class="col-md-4 text-center">
          <img src={speaker.image} alt={speaker.name} class="rounded-circle img-fluid mb-3" style="width: 150px; height: 150px;">
          <h5>{speaker.name}</h5>
          <p class="text-muted">{speaker.title}</p>
        </div>
      {/each}
    </div>
  </div>
</section>
