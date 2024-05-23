<template>
  <nav class="navbar">
    <div class="navbar-brand">Koffee Shop</div>
    <ul class="navbar-nav">
      <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Menu</a></li>
      <li class="nav-item"><a class="nav-link" href="#">About</a></li>
      <li class="nav-item"><a class="nav-link" href="#">Contact</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
};
</script>

<style>
.navbar {
  display: flex;
  justify-content: space-between;
  padding: 10px 20px;
  background-color: #4A2C2A;
  color: #fff;
}
.navbar-brand {
  font-size: 1.5em;
  font-weight: bold;
}
.navbar-nav {
  display: flex;
  list-style: none;
}
.nav-item {
  margin: 0 10px;
}
.nav-link {
  color: #fff;
  text-decoration: none;
}
.nav-link:hover {
  text-decoration: underline;
}
</style>
