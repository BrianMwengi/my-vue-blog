<template>
  <header class="header">
    <nav class="navbar">
      <div class="navbar-container">
        <div class="logo">My Vue Blog</div>
        <div class="nav-links">
          <router-link to="/">Home</router-link>
          <router-link to="/about">About</router-link>
          <router-link to="/blog">Blog</router-link>
          <router-link to="/contact">Contact</router-link>
        </div>
      </div>
    </nav>
  </header>
</template>

<script setup lang="ts">
// Navbar component
</script>

<style scoped>
.header {
  width: 100%;
  position: sticky;
  top: 0;
  z-index: 100;
  background-color: #2c3e50;
}

.navbar {
  width: 100%;
}

.navbar-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}

.logo {
  font-weight: bold;
  font-size: 1.5rem;
  color: white;
}

.nav-links {
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  padding: 0.5rem;
  transition: all 0.3s ease;
}

.nav-links a:hover {
  color: #41b883;
}

.nav-links a.router-link-active {
  font-weight: bold;
  border-bottom: 2px solid #41b883;
  color: #41b883;
}

@media (max-width: 768px) {
  .navbar-container {
    flex-direction: column;
    gap: 1rem;
    padding: 1rem;
  }
  
  .nav-links {
    width: 100%;
    justify-content: space-between;
  }
}
</style>