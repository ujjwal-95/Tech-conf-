<script>
  export let sponsors = [
    { name: "Google", logo: "/googleimg.jpg", url: "https://www.google.com" },
    { name: "Microsoft", logo: "/microsoftimg.jpg", url: "https://www.microsoft.com" },
    { name: "Amazon", logo: "/amazonimg.jpg", url: "https://www.amazon.com" },
    { name: "Meta", logo: "/metaimg.jpg", url: "https://www.meta.com" },
    { name: "Tesla", logo: "/teslaimg.jpg", url: "https://www.tesla.com" },
    { name: "IBM", logo: "/ibmimg.jpg", url: "https://www.ibm.com" }
  ];
</script>

<section class="py-5">
  <div class="container text-center">
    <h2 class="mb-4">Our Sponsors</h2>
    <div class="row justify-content-center">
      {#each sponsors as sponsor}
        <div class="col-6 col-md-4 col-lg-2 mb-4 d-flex align-items-center justify-content-center">
          <a href={sponsor.url} target="_blank">
            <img src={sponsor.logo} alt={sponsor.name} class="img-fluid p-2 border rounded shadow"
                 style="width: 150px; height: 100px; object-fit: contain;">
          </a>
        </div>
      {/each}
    </div>
  </div>
</section>
