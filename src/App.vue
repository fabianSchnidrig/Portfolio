<template>
  <header class="navbar">
    <h2 class="logo">Fabian</h2>

    <nav>
      <RouterLink to="/">Home</RouterLink>
<RouterLink to="/about">About</RouterLink>
<RouterLink to="/skills">Skills</RouterLink>
<RouterLink to="/contact">Contact</RouterLink>

    </nav>
  </header>

  <main class="page">
    <RouterView />
  </main>
</template>

<style scoped>
.navbar {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 10%;
  background: #0a0a0a;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo {
  color: #00bcd4;
  font-weight: 700;
}

nav a {
  margin-left: 20px;
  color: white;
  text-decoration: none;
  font-weight: 600;
}

nav a.router-link-exact-active {
  color: #00bcd4;
}

.page {
  width: 100%;
  overflow-x: hidden;
}
</style>
