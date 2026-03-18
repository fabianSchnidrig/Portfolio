<template>
  <section class="about">
    <div class="about-container">
      <h2>About <span>Me</span></h2>
      <h3>Platform IT Apprentice</h3>

      <p>
        I'm Fabian, a platform IT apprentice with a strong interest in web development 
        and server environments. I enjoy building modern applications, experimenting 
        with new technologies, and improving systems step by step.
      </p>

      <p>
        My background in different fields has helped me develop strong problem-solving 
        skills and adaptability. I am motivated to continuously learn and grow in the 
        IT world.
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
  min-height: calc(100vh - 90px);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 10%;
  text-align: center;
}

.about-container {
  max-width: 700px;
}

.about h2 {
  font-size: 3rem;
  margin-bottom: 10px;
}

.about h2 span {
  color: #00bcd4;
}

.about h3 {
  font-size: 1.6rem;
  color: #00bcd4;
  margin-bottom: 25px;
}

.about p {
  font-size: 1.1rem;
  line-height: 1.8;
  color: #c0c0c0;
  margin-bottom: 20px;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 12px 28px;
  background: #00bcd4;
  color: #111;
  text-decoration: none;
  font-weight: 600;
  border-radius: 8px;
  transition: 0.3s;
}

.btn:hover {
  background: #00d4ee;
}
</style>