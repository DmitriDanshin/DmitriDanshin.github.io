<template>
  <div class="portfolio__wrapper">

    <a v-for="grid in grids" :key="grid" :href="grid.href" class="portfolio__item"><img :src="grid.img"
                                                                                                 alt="img"></a>
  </div>
</template>

<script>
export default {
  name: "Works-grid",
  props: {
    grids: {
      type: Array,
      required: true
    }
  }
}
</script>

<style scoped>

</style>