<template>
  <div id="app">
    <nav class="navbar">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>

    <main>
      <RouterView/>
    </main>
  </div>
</template>

<style>
body {
  margin: 0;
  font-family: system-ui, sans-serif;
  background-color: #f0f4f8;
}

.navbar {
  display: flex;
  gap: 1.5rem;
  padding: 1rem 2rem;
  background-color: #1e3a5f;
}

.navbar a {
  color: #e0f2fe;
  text-decoration: none;
  font-weight: 500;
  padding: 0.4rem 0.8rem;
  border-radius: 6px;
  transition: background-color 0.2s;
}

.navbar a:hover,
.navbar a.router-link-active {
  background-color: #3b82f6;
  color: white;
}

.page {
  padding: 2rem;
  max-width: 800px;
  margin: 0 auto;
}

h1 {
  color: #1e3a5f;
}
</style>