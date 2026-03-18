<template>
  <section class="contact">
    <div class="contact-container">
      <h2>Contact <span>Me</span></h2>
      <p class="contact-text">
        You can reach out to me anytime — I will get back to you as soon as possible.
      </p>

      <form class="contact-form">
        <div class="form-group">
          <label for="name">Name</label>
          <input id="name" type="text" placeholder="Your name" />
        </div>

        <div class="form-group">
          <label for="email">E-mail</label>
          <input id="email" type="email" placeholder="your@email.com" />
        </div>

        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" rows="5" placeholder="Your message"></textarea>
        </div>

        <button type="submit" class="btn">Send Message</button>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactView",
};
</script>

<style scoped>
.contact {
  min-height: calc(100vh - 86px);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 110px 20px 40px;
  background: #0a0a0a;
}

.contact-container {
  width: 100%;
  max-width: 720px;
  text-align: center;
}

.contact h2 {
  font-size: 3rem;
  margin-bottom: 12px;
  color: #eaeaea;
}

.contact h2 span {
  color: #00bcd4;
}

.contact-text {
  color: #bdbdbd;
  font-size: 1.1rem;
  line-height: 1.7;
  margin-bottom: 36px;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 22px;
  text-align: left;
}

.form-group {
  display: flex;
  flex-direction: column;
}

.form-group label {
  margin-bottom: 10px;
  color: #e0e0e0;
  font-size: 1rem;
  font-weight: 500;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 16px 18px;
  border-radius: 10px;
  border: 2px solid #1f1f1f;
  background: #111;
  color: white;
  font-size: 1rem;
  box-sizing: border-box;
  outline: none;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
}

.form-group input::placeholder,
.form-group textarea::placeholder {
  color: #8a8a8a;
}

.form-group input:focus,
.form-group textarea:focus {
  border-color: #00bcd4;
  box-shadow: 0 0 12px rgba(0, 188, 212, 0.2);
}

.form-group textarea {
  resize: vertical;
  min-height: 140px;
}

.btn {
  align-self: center;
  margin-top: 10px;
  padding: 14px 34px;
  background: #00bcd4;
  color: #111;
  border: 2px solid #00bcd4;
  border-radius: 8px;
  font-size: 1rem;
  font-weight: 700;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn:hover {
  background: transparent;
  color: #00bcd4;
  box-shadow: 0 0 18px rgba(0, 188, 212, 0.35);
  transform: translateY(-2px);
}

@media (max-width: 768px) {
  .contact {
    padding: 110px 16px 40px;
  }

  .contact h2 {
    font-size: 2.4rem;
  }

  .contact-text {
    font-size: 1rem;
  }
}
</style>