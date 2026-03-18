<template>
  <header class="navbar">
    <h2 class="logo">Fabian</h2>

    <nav class="nav-links">
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
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 86px;
  background: #0a0a0a;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 50px;
  box-sizing: border-box;
  z-index: 1000;
  border-bottom: 2px solid #00bcd4;
}

.logo {
  color: #00bcd4;
  font-weight: 700;
  font-size: 2rem;
  letter-spacing: 0.5px;
}

.nav-links {
  display: flex;
  align-items: center;
}

.nav-links a {
  margin-left: 34px;
  color: white;
  text-decoration: none;
  font-weight: 600;
  font-size: 1.15rem;
  position: relative;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #00bcd4;
}

.nav-links a::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -7px;
  width: 0;
  height: 2px;
  background: #00bcd4;
  transition: width 0.3s ease;
}

.nav-links a:hover::after,
.nav-links a.router-link-exact-active::after {
  width: 100%;
}

.nav-links a.router-link-exact-active {
  color: #00bcd4;
}

.page {
  width: 100%;
  max-width: none;
  margin: 0;
  padding: 0;
}

@media (max-width: 768px) {
  .navbar {
    height: auto;
    padding: 18px 24px;
    flex-direction: column;
    gap: 14px;
  }

  .logo {
    font-size: 1.7rem;
  }

  .nav-links {
    flex-wrap: wrap;
    justify-content: center;
  }

  .nav-links a {
    margin: 0 12px;
    font-size: 1rem;
  }
}
</style>