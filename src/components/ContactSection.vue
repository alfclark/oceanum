<template>
  <div style="margin-top: -50px; position: absolute" id="contact"></div>
  <section class="contact">
    <div class="animation">
      <h3>Tú tambien puedes ayudar. ¡Contáctanos!</h3>
      <p>Ubicación: Mexico</p>
    </div>
    <div class="form">
      <form
        class="row g-3"
        ref="anyName"
        @submit="submitForm"
        autocomplete="off"
        action="https://formsubmit.co/9144a6a93c855ef6560bfe2b18cdbc55"
        method="POST"
      >
        <!-- Configs -->
        <input type="text" name="_honey" style="display: none" />
        <input type="hidden" name="_captcha" value="false" />
        <input type="hidden" name="_next" value="#" />
        <input
          type="hidden"
          name="_subject"
          value="Nuevo mensaje de contacto!"
        />
        <!-- Inputs -->
        <input
          type="text"
          name="name"
          v-model="name"
          placeholder="Tu nombre"
          required
        />
        <input
          type="email"
          name="email"
          v-model="email"
          placeholder="tu_correo@email.com"
          required
        />
        <label for="reason">Razón de contacto:</label>
        <select name="reason" v-model="reason">
          <option value="professional">Donación</option>
          <option value="education">Sponsor</option>
          <option value="feedback">Cuidados</option>
        </select>
        <input
          type="text"
          name="message"
          v-model="message"
          placeholder="Mensaje"
          required
          cols="30"
          rows="5"
        />
        <button class="button" :class="hide" type="submit">Enviar</button>
        <div class="sent" :class="show">
          ¡Enviado! <i class="fa-solid fa-check"></i>
        </div>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    submitForm() {
      this.$refs.anyName.reset();
      const btnStatus = "hide";
      const sentStatus = "show";
      this.hide = btnStatus;
      this.show = sentStatus;
    },
  },
  data() {
    return {
      hide: "",
      show: "",
    };
  },
};
</script>

<style scoped>
.contact {
  display: flex;
  height: 100%;
  padding: 0;
  margin: 3rem 0;
  left: 0;
}
.animation {
  display: flex;
  flex-direction: column;
  position: relative;
  width: 30vw;
  height: 100%;
  text-align: left;
  padding-left: 1rem;
  color: var(--carbon);
}
.animation h3 {
  font-size: 2rem;
  margin-bottom: 3rem;
}
.animation p {
  margin: 0;
  margin-bottom: 1rem;
}

.form form {
  width: 70vw;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 0 2rem;
}

label {
  margin-top: 1rem;
  color: var(--carbon);
}
input,
select {
  margin-top: 1rem;
  height: 65px;
  width: 100%;
  border: 2px solid var(--water);
  background: var(--dark);
  padding: 0 1.5rem;
  border-radius: 15px;
  outline: none;
  font-weight: 400;
  font-size: 1rem;
  color: var(--black);
}

::placeholder {
  color: rgba(31, 26, 26, 0.491);
}

.button {
  margin: 1rem 0;
  padding: 0.5rem 3rem;
  background-color: var(--orange);
  color: var(--black);
  border: solid var(--sand);
  border-radius: 2rem;
}
.button:hover {
  background-color: var(--orangeDark);
  color: var(--black);
  transition: 0.4s;
}
.sent {
  margin: 1rem 0;
  padding: 0.5rem 3rem;
  background-color: rgb(64, 134, 64);
  color: white;
  border: solid rgb(64, 134, 64);
  border-radius: 2rem;
  display: none;
}
.hide {
  display: none;
  transition: 1s;
}
.show {
  display: block;
  transition: 1s;
}

@media screen and (max-width: 900px) {
  .contact {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .animation {
    width: 80vw;
    text-align: center;
    padding-left: 0;
    margin: 0;
  }

  .animation h3 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }
  .animation p {
    font-size: 0.7rem;
  }
}
</style>
