<!-- Navbar.svelte -->
<header class="navbar">
  <img src="logo_name.svg" alt="Company Logo" class="logo">
  <nav>
    <ul class="nav-list">
      <li class="nav-item"><a href="#">Home</a></li>
      <li class="nav-item"><a href="#">About</a></li>
      <li class="nav-item"><a href="#">Contact</a></li>
    </ul>
  </nav>
</header>

<style>
  .navbar {
    display: flex;
    align-items: center;
    padding: 10px;
    background-color: #f1f1f1;
  }

  .logo {
    height: 40px;
    margin-right: 10px;
  }

  .nav-list {
    list-style: none;
    display: flex;
  }

  .nav-item {
    margin-right: 10px;
  }

  .nav-item a {
    text-decoration: none;
    color: #333;
    font-weight: bold;
  }
</style>
