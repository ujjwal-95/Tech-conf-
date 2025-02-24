<script>
  let name = "";
  let email = "";
  let message = "";

  function handleSubmit() {
    alert(`Thank you, ${name}! We have received your message.`);
    name = "";
    email = "";
    message = "";
  }
</script>

<div class="container mt-5">
  <h2 class="text-center mb-4">Contact Us</h2>

  <div class="row justify-content-center">
    <div class="col-md-6">
      <form on:submit|preventDefault={handleSubmit}>
        <div class="mb-3">
          <label for="name" class="form-label">Name</label>
          <input type="text" id="name" class="form-control" bind:value={name} required />
        </div>

        <div class="mb-3">
          <label for="email" class="form-label">Email</label>
          <input type="email" id="email" class="form-control" bind:value={email} required />
        </div>

        <div class="mb-3">
          <label for="message" class="form-label">Message</label>
          <textarea id="message" class="form-control" rows="4" bind:value={message} required></textarea>
        </div>

        <button type="submit" class="btn btn-primary w-100">Send Message</button>
      </form>
    </div>
  </div>

  <!-- Social Media Links -->
  <div class="text-center mt-4">
    <h5>Follow Us On</h5>
    <a href="/" class="me-3" aria-label="Facebook"><i class="bi bi-facebook fs-3"></i></a>
    <a href="/" class="me-3" aria-label="Twitter"><i class="bi bi-twitter-x fs-3"></i></a>
    <a href="/" class="me-3" aria-label="LinkedIn"><i class="bi bi-linkedin fs-3"></i></a>
    <a href="/" aria-label="Instagram"><i class="bi bi-instagram fs-3"></i></a>
  </div>
    

</div>
