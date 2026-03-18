<template>
  <section class="home">
    <div class="home-content">
      <p class="intro">Hello, I'm</p>
      <h1>Fabian</h1>
      <h2>Platform IT Apprentice</h2>

      <p class="description">
        I am a platform IT apprentice passionate about building modern web applications
        and working with server infrastructures. I enjoy learning new technologies,
        optimizing workflows, and continuously improving my skills in both development
        and system administration.
      </p>

      <div class="buttons">
        <router-link to="/about" class="btn btn-primary">About Me</router-link>
        <a href="/CV.pdf" class="btn btn-outline" download>Download CV</a>
      </div>
    </div>

    <div class="home-image">
      <img src="@/assets/images/profilbild.png" alt="Fabian Hero" />
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
  min-height: calc(100vh - 70px);
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 0 0 8%;
  background: #111;
  color: white;
  overflow: hidden;
  box-sizing: border-box;
}

.home-content {
  flex: 0 0 38%;
  max-width: 520px;
  z-index: 2;
}

.intro {
  font-size: 2.2rem;
  color: #d6d6d6;
  margin: 0 0 8px;
}

.home-content h1 {
  font-size: 4rem;
  line-height: 1.05;
  margin: 0 0 14px;
  color: #00bcd4;
  text-shadow: 0 0 10px rgba(0, 188, 212, 0.2);
}

.home-content h2 {
  font-size: 2.2rem;
  color: #ffffff;
  margin: 0 0 22px;
}

.description {
  font-size: 1.1rem;
  line-height: 1.8;
  color: #c0c0c0;
  max-width: 500px;
  margin-bottom: 36px;
}
.buttons {
  display: flex;
  gap: 18px;
  flex-wrap: wrap;
  margin-top: 10px;
}
.btn {
  display: inline-block;
  padding: 14px 28px;
  text-decoration: none;
  font-weight: 700;
  border-radius: 8px;
  border: 2px solid #00bcd4;
  transition: all 0.3s ease;
}

.btn-primary {
  background: #00bcd4;
  color: #111;
}

.btn-primary:hover {
  background: #00d4ee;
  color: #111;
  transform: translateY(-2px);
  box-shadow: 0 0 18px rgba(0, 188, 212, 0.35);
}

.btn-outline {
  background: transparent;
  color: #00bcd4;
}

.btn-outline:hover {
  background: #00bcd4;
  color: #111;
  transform: translateY(-2px);
  box-shadow: 0 0 18px rgba(0, 188, 212, 0.35);
}

.home-image {
  flex: 0 0 62%;
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  min-width: 0;
  height: 100%;
  z-index: 1;

  position: relative;
  /* 🔥 hinzufügen */
}

.home-image::before {
  content: "";
  position: absolute;
  left: -200px;
  top: 0;
  width: 300px;
  height: 100%;
  background: linear-gradient(to right, #111, transparent);
  z-index: 2;
}

.home-image img {
  width: 65vw;
  max-width: none;
  max-height: 95vh;
  height: auto;
  display: block;

  transform: translateX(80px);
  /* 👉 nach rechts schieben */
}

.intro {
  font-size: 1.6rem;
  color: #a0a0a0;
}

@media (max-width: 1100px) {
  .home-content h1 {
    font-size: 4rem;
  }

  .home-content h2 {
    font-size: 1.9rem;
  }

  .home-image img {
    width: 52vw;
  }
}

@media (max-width: 900px) {
  .home {
    flex-direction: column-reverse;
    text-align: center;
    padding: 40px 6% 50px;
    gap: 20px;
  }

  .home-content {
    max-width: 100%;
    flex: unset;
  }

  .home-content h1 {
    font-size: 3rem;
  }

  .home-content h2 {
    font-size: 1.5rem;
  }

  .buttons {
    justify-content: center;
  }

  .home-image {
    justify-content: center;
    align-items: center;
    min-width: auto;
    flex: unset;
  }

  .home-image img {
    width: min(420px, 90vw);
    max-height: 45vh;
  }
}
</style>