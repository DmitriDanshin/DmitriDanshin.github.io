<template>
  <section class="promo">
    <div class="hamburger" @click="open">

      <span></span>
      <span class="long"></span>
      <span></span>

    </div>
    <div class="container">
      <div class="title title_fz16 promo__subtitle">My name is Dima</div>
      <h1 class="title title_fz48 promot__title">I am a web developer
        from Krasnodar</h1>
      <div class="promo__btns">
        <a href="#" class="promo__link btn">Portfolio</a>
        <a href="#" class="promo__link">About me</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Promo-block",
  emits: {
    "open-menu": null,
  },

  methods: {
    open() {
      this.$emit('open-menu');

    },
  }
}
</script>

<style scoped>

</style>