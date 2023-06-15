<!-- Login.svelte -->
<script>
  export let selectedOption;
</script>

<main>
  <h1>Login to your account</h1>
  <form>
    <label for="username"><b>Username</b></label>
    <input type="text" placeholder="Enter Username" name="username" required>

    <label for="password"><b>Password</b></label>
    <input type="password" placeholder="Enter Password" name="password" required>

    <button type="submit">Login</button>
    <label>
      <input type="checkbox" checked="checked" name="remember"> Remember me
    </label>
  </form>
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

  form {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  label {
    margin-top: 10px;
  }

  input {
    margin-top: 5px;
    padding: 8px;
    font-size: 16px;
    width: 200px;
    border-radius: 4px;
    border: 1px solid #ccc;
  }

  button {
    margin-top: 10px;
    padding: 10px 20px;
    font-size: 16px;
    border: none;
    border-radius: 4px;
    background-color: #4CAF50;
    color: white;
    cursor: pointer;
  }

  button:hover {
    background-color: #45a049;
  }

  input[type="checkbox"] {
    margin-top: 10px;
  }
</style>
