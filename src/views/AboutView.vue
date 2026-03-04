<template>
  <section class="about">
    <div class="about-img">
      <img src="@/assets/images/images_silhouette.jpg" alt="About Image" />
    </div>

    <div class="about-content">
      <h2>About Me</h2>
      <h3>IT Apprentice & Developer</h3>

      <p>
        I'm Fabian, an IT apprentice specializing in platform development.
        I enjoy building modern web applications, experimenting with server
        environments, and optimizing workflows. My background in construction
        and healthcare gives me a unique perspective on problem‑solving and
        teamwork.
      </p>

      <p>
        I love learning new technologies, working on personal hardware projects,
        and improving my development skills step by step.
      </p>

      <router-link to="/skills" class="btn">My Skills</router-link>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutView",
};
</script>

<style scoped>
.about {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 80px 10%;
  min-height: 100vh;
  background: #111;
  color: white;
  gap: 40px;
}

.about-img img {
  width: 350px;
  border-radius: 12px;
  border: 4px solid #00bcd4;
}

.about-content {
  max-width: 600px;
}

.about-content h2 {
  font-size: 42px;
  margin-bottom: 10px;
}

.about-content h3 {
  font-size: 24px;
  color: #00bcd4;
  margin-bottom: 20px;
}

.about-content p {
  font-size: 18px;
  line-height: 1.6;
  margin-bottom: 20px;
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
</style>
