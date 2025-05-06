<template>
  <footer class="footer">
    <div class="footer-container">
      <p>&copy; {{ currentYear }} My Vue Blog. All rights reserved.</p>
    </div>
  </footer>
</template>

<script setup lang="ts">
const currentYear = new Date().getFullYear();
</script>

<style scoped>
.footer {
  background-color: #2c3e50;
  color: white;
  width: 100%;
  padding: 1.5rem 0;
  margin-top: auto; /* This helps push the footer down */
}

.footer-container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
  padding: 0 2rem;
}
</style>