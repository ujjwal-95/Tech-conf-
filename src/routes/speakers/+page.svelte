<script>
  export let speakers = [
    { name: "John Doe", title: "AI Researcher", bio: "Expert in AI and ML, with 10+ years of experience.", image: "/expert1.jpg" },
    { name: "Jane Smith", title: "Cybersecurity Expert", bio: "Specialist in data security and ethical hacking.", image: "/expert2.jpg" },
    { name: "Alice Johnson", title: "Blockchain Developer", bio: "Pioneer in decentralized technologies and crypto.", image: "/expert3.png" },
    { name: "Robert Brown", title: "Cloud Architect", bio: "Designing scalable cloud solutions for enterprises.", image: "/expert4.jpg" },
    { name: "Emily Davis", title: "Data Scientist", bio: "Turning data into insights with AI & analytics.", image: "/expert5.jpg" },
    { name: "Michael Lee", title: "IoT Specialist", bio: "Innovating in smart devices and edge computing.", image: "/expert6.jpg" },
    { name: "Sophia White", title: "Quantum Computing Engineer", bio: "Exploring the future of quantum algorithms.", image: "/expert7.jpg" }
  ];
</script>

<section class="py-5 bg-light">
  <div class="container">
    <h2 class="text-center mb-4">Meet Our Speakers</h2>
    <div class="row">
      {#each speakers as speaker}
        <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
          <div class="card text-center shadow-sm">
            <img src={speaker.image} alt={speaker.name} class="rounded-circle mx-auto mt-3" style="width: 120px; height: 120px;">
            <div class="card-body">
              <h5 class="card-title">{speaker.name}</h5>
              <p class="text-muted">{speaker.title}</p>
              <p class="card-text">{speaker.bio}</p>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
