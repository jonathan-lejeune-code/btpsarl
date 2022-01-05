<template>
  <v-container>
    <h1>Contact</h1>
    <p>Pour toute question vous pouvez nous contacter :</p>
    <h2>Siége social</h2>
    <div class="googlemap">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2139.975173486406!2d2.2642039973260215!3d48.96406862440712!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66639288a0cc9%3A0xf7c12db01477f41d!2s30%20Rue%20Jean%20Coquelin%2C%2095110%20Sannois!5e0!3m2!1sfr!2sfr!4v1641400475732!5m2!1sfr!2sfr"
        width="100%"
        height="450"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
      ></iframe>
    </div>

    <h2 class="mt-10">Par mail</h2>
    <v-btn
      color="orange"
      class="mr-4 mt-5 white--text"
      href="mailto:?subject=Question du site"
      >Envoyé un mail</v-btn
    >
    <h2 class="mt-10">Par téléphone</h2>
    <p>01-02-02-02-02</p>
  </v-container>
</template>

<script>
export default {
  name: 'ContactPage',
}
</script>

<style></style>
