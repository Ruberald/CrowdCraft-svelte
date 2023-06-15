<!-- LandingPage.svelte -->
<script>
  export let selectOption;
</script>

<main>
  <h1>What describes you best?</h1>
  <p>Please select an option:</p>
  <div class="options">
    <button on:click={() => selectOption('hoster')}>Hoster</button>
    <button on:click={() => selectOption('attendee')}>Attendee</button>
  </div>
</main>

<style>

  @font-face {
      font-family: 'Bree Serif';
      src: url('/fonts/BreeSerif-Regular.ttf') format('truetype');
      /* Add more font formats here if you have them */
      /* e.g., src: url('/fonts/BreeSerif-Regular.woff2') format('woff2'),
                    url('/fonts/BreeSerif-Regular.woff') format('woff'); */
    }


  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    text-align: center;
    font-family: 'Bree Serif', Arial, sans-serif;
  }

  .options {
    margin-top: 20px;
  }

  button {
    margin: 5px;
    padding: 10px 20px;
    font-size: 16px;
  }
</style>
