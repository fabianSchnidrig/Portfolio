<template>
  <section class="home">
    <div class="home-content">
      <h1>Hi, I'm Fabian</h1>
      <h3>IT Apprentice & Developer</h3>
      <p>
        I build modern web applications, experiment with server environments,
        and love optimizing workflows. Welcome to my portfolio!
      </p>

      <div class="buttons">
        <router-link to="/about" class="btn">About Me</router-link>
        <a href="/CV.pdf" class="btn" download>Download CV</a>
      </div>
    </div>

    <div class="home-img">
      <img src="@/assets/images/pngegg.jpg" alt="Profile" />
    </div>
  </section>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>
.home {
  min-height: calc(100vh - 90px);
  /* Platz für Navbar */
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 10%;
  box-sizing: border-box;
}

.home-content {
  max-width: 600px;
}

.home-content h1 {
  font-size: 48px;
  margin-bottom: 10px;
}

.home-content h3 {
  font-size: 28px;
  color: #00bcd4;
  margin-bottom: 20px;
}

.home-content p {
  font-size: 18px;
  line-height: 1.6;
  margin-bottom: 30px;
}

.buttons {
  display: flex;
  gap: 20px;
}

.btn {
  padding: 12px 24px;
  background: #00bcd4;
  color: black;
  text-decoration: none;
  font-weight: 600;
  border-radius: 6px;
  transition: 0.3s;
}

.btn:hover {
  background: #0097a7;
}

.home-img img {
  max-width: 100%;
  width: 320px;
  border-radius: 50%;
  border: 4px solid #00bcd4;
}


@media (max-width: 900px) {
  .home {
    flex-direction: column;
    text-align: center;
    height: auto;
    padding: 40px 5%;
  }

  .home-img img {
    width: 250px;
    margin-top: 30px;
  }
}
</style>
