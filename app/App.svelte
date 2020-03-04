<script>
  const cardio = ["swimming", "biking", "running", "boxing", "HIIT"];
  const upperBody = ["shoulder raises", "bicep curls", "bench press", "trx row"];
  const lowerBody = ["leg press", "squats", "lunges", "sled pushes"];
  let randomCardio;
  let randomUpperBody;
  let randomLowerBody;

  function tapForCardio() {
    randomCardio = cardio[Math.floor(Math.random() * cardio.length)];
  }

  function tapForUpperBody() {
    randomUpperBody = cardio[Math.floor(Math.random() * upperBody.length)];
  }

  function tapForLowerBody() {
    randomLowerBody= cardio[Math.floor(Math.random() * lowerBody.length)];
  }
</script> 

<page>
  <actionBar title="My App" icon="" />
  <stackLayout class="p-20">
    <label text="Tap the button for cardio" class="h1 text-center" />
    <button text="TAP" on:tap={tapForCardio} class="-primary -active" />
    <label text={randomCardio} class="h2 text-center" textWrap="true" />

      <label text="Tap the button for upperBody" class="h1 text-center" />
    <button text="TAP" on:tap={tapForUpperBody} class="-primary -active" />
    <label text={randomUpperBody} class="h2 text-center" textWrap="true" />

      <label text="Tap the button for lowerBody" class="h1 text-center" />
    <button text="TAP" on:tap={tapForLowerBody} class="-primary -active" />
    <label text={randomLowerBody} class="h2 text-center" textWrap="true" />
    
  </stackLayout>
</page>

