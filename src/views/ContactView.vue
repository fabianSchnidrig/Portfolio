<script setup lang="ts">
</script>

<template>
  <section class="contact">
    <h1>Kontakt</h1>
    <p>Du kannst mich jederzeit erreichen – ich melde mich so schnell wie möglich.</p>

    <form class="contact-form">
      <label>
        Name
        <input type="text" placeholder="Dein Name" />
      </label>

      <label>
        E-Mail
        <input type="email" placeholder="deine@mail.ch" />
      </label>

      <label>
        Nachricht
        <textarea placeholder="Deine Nachricht"></textarea>
      </label>

      <button type="submit">Senden</button>
    </form>
  </section>
</template>

<style scoped>
.contact {
  max-width: 600px;
  margin: 0 auto;
  padding: 2rem;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

input,
textarea {
  width: 100%;
  padding: .7rem;
  border-radius: 6px;
  border: 1px solid #ccc;
}

button {
  padding: .8rem;
  border: none;
  background: #42b883;
  color: white;
  border-radius: 6px;
  cursor: pointer;
}
</style>
