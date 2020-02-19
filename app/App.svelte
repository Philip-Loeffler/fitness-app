<script>
  const cardio = ["swimming", "biking", "running", "boxing", "HIIT"];

  let randomWork;

  function tapForCardio() {
    randomWork = cardio[Math.floor(Math.random() * cardio.length)];
  }
</script>

<page>
  <actionBar title="My App" icon="" />
  <stackLayout class="p-20">
    <label text="Tap the button" class="h1 text-center" />
    <button text="TAP" on:tap={tapForCardio} class="-primary -active" />
    <label text={randomWork} class="h2 text-center" textWrap="true" />
  </stackLayout>
</page>
