<template>
  <section class="portfolio">
    <div class="container">

      <h3 class="title title_fz36 title__section-subtitle">
        My works
      </h3>
      <div class="divider"></div>

      <div class="portfolio__menu">
        <svg @click="openGrid" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="th"
             class="svg-inline--fa fa-th fa-w-16 portfolio__icon  " role="img"
             :class="{active: isGridOpen}"
             xmlns="http://www.w3.org/2000/svg"
             viewBox="0 0 512 512">
          <path fill="currentColor"
                d="M149.333 56v80c0 13.255-10.745 24-24 24H24c-13.255 0-24-10.745-24-24V56c0-13.255 10.745-24 24-24h101.333c13.255 0 24 10.745 24 24zm181.334 240v-80c0-13.255-10.745-24-24-24H205.333c-13.255 0-24 10.745-24 24v80c0 13.255 10.745 24 24 24h101.333c13.256 0 24.001-10.745 24.001-24zm32-240v80c0 13.255 10.745 24 24 24H488c13.255 0 24-10.745 24-24V56c0-13.255-10.745-24-24-24H386.667c-13.255 0-24 10.745-24 24zm-32 80V56c0-13.255-10.745-24-24-24H205.333c-13.255 0-24 10.745-24 24v80c0 13.255 10.745 24 24 24h101.333c13.256 0 24.001-10.745 24.001-24zm-205.334 56H24c-13.255 0-24 10.745-24 24v80c0 13.255 10.745 24 24 24h101.333c13.255 0 24-10.745 24-24v-80c0-13.255-10.745-24-24-24zM0 376v80c0 13.255 10.745 24 24 24h101.333c13.255 0 24-10.745 24-24v-80c0-13.255-10.745-24-24-24H24c-13.255 0-24 10.745-24 24zm386.667-56H488c13.255 0 24-10.745 24-24v-80c0-13.255-10.745-24-24-24H386.667c-13.255 0-24 10.745-24 24v80c0 13.255 10.745 24 24 24zm0 160H488c13.255 0 24-10.745 24-24v-80c0-13.255-10.745-24-24-24H386.667c-13.255 0-24 10.745-24 24v80c0 13.255 10.745 24 24 24zM181.333 376v80c0 13.255 10.745 24 24 24h101.333c13.255 0 24-10.745 24-24v-80c0-13.255-10.745-24-24-24H205.333c-13.255 0-24 10.745-24 24z"></path>
        </svg>

        <svg @click="openCarousel"  :class="{active: isCarouselOpen}" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="square"
             class="svg-inline--fa fa-square fa-w-14 portfolio__icon  " role="img"
             xmlns="http://www.w3.org/2000/svg"
             viewBox="0 0 448 512">
          <path fill="currentColor"
                d="M400 32H48C21.5 32 0 53.5 0 80v352c0 26.5 21.5 48 48 48h352c26.5 0 48-21.5 48-48V80c0-26.5-21.5-48-48-48z"></path>
        </svg>
      </div>
      <div class="divider"></div>
      <works-grid v-if="isGridOpen" :grids="works"/>
      <works-carousel v-if="isCarouselOpen" :sliders="works"/>
    </div>
  </section>
</template>

<script>
import WorksGrid from "./Works-grid";
import WorksCarousel from "./Works-carousel";

export default {
  name: "Works-block",
  components: {WorksCarousel, WorksGrid},
  data() {
    return {
      isGridOpen: false,
      isCarouselOpen: true,
      works: [
        {
          img: require("../../assets/images/works/uber.jpg"),
          href: '#',
        },
        {
          img: require("../../assets/images/works/bread.jpg"),
          href: '#',
        },
        {
          img: require("../../assets/images/works/uber.jpg"),
          href: '#',
        },
        {
          img: require("../../assets/images/works/pulse.jpg"),
          href: '#',
        },
        {
          img: require("../../assets/images/works/uber.jpg"),
          href: '#',
        },
        {
          img: require("../../assets/images/works/pulse.jpg"),
          href: '#',
        },
        {
          img: require("../../assets/images/works/ipad.jpg"),
          href: '#',
        }, {
          img: require("../../assets/images/works/ipad.jpg"),
          href: '#',
        },

      ],
    }
  },
  methods: {
    openGrid() {
      this.isGridOpen = true;
      this.isCarouselOpen = false;
    },
    openCarousel() {
      this.isGridOpen = false;
      this.isCarouselOpen = true;
    }
  }
}
</script>

<style scoped>

</style>