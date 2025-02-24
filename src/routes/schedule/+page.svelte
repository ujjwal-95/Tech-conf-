<script>
  export let schedule = [
    { date: "March 10, 2025", time: "10:00 AM - 11:00 AM", topic: "The Future of AI", speaker: "John Doe" },
    { date: "March 10, 2025", time: "11:30 AM - 12:30 PM", topic: "Cybersecurity in 2025", speaker: "Jane Smith" },
    { date: "March 10, 2025", time: "2:00 PM - 3:00 PM", topic: "Blockchain Innovations", speaker: "Alice Johnson" },
    { date: "March 11, 2025", time: "10:00 AM - 11:00 AM", topic: "Cloud Computing Trends", speaker: "Robert Brown" },
    { date: "March 11, 2025", time: "11:30 AM - 12:30 PM", topic: "Data Science for Business", speaker: "Emily Davis" },
    { date: "March 11, 2025", time: "2:00 PM - 3:00 PM", topic: "IoT and Smart Cities", speaker: "Michael Lee" },
    { date: "March 12, 2025", time: "10:00 AM - 11:00 AM", topic: "Quantum Computing Revolution", speaker: "Sophia White" }
  ];
</script>

<section class="py-5">
  <div class="container">
    <h2 class="text-center mb-4">Conference Schedule</h2>
    <div class="table-responsive">
      <table class="table table-striped table-bordered">
        <thead class="table-dark text-center">
          <tr>
            <th>Date</th>
            <th>Time</th>
            <th>Topic</th>
            <th>Speaker</th>
          </tr>
        </thead>
        <tbody>
          {#each schedule as session}
            <tr>
              <td>{session.date}</td>
              <td>{session.time}</td>
              <td>{session.topic}</td>
              <td>{session.speaker}</td>
            </tr>
          {/each}
        </tbody>
      </table>
    </div>
  </div>
</section>
