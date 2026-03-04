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
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 80px 10%;
  min-height: 100vh;
  background: #0f0f0f;
  color: white;
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
  width: 350px;
  border-radius: 50%;
  border: 4px solid #00bcd4;
}
</style>
