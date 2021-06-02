<template>

  <promo-block @open-menu="open"/>
  <menu-block :isMenuOpen="isMenuOpen" @close-menu="close"/>
  <about-block/>
  <works-block/>
  <skills-block/>
  <resume-block/>
  <contacts-block/>


</template>

<script>

import AboutBlock from "./components/about/About-block";
import ContactsBlock from "@/components/contacts/Contacts-block";
import PromoBlock from "@/components/promo/Promo-block";
import WorksBlock from "@/components/works/Works-block";
import SkillsBlock from "@/components/skills/Skills-block";
import MenuBlock from "@/components/menu/Menu-block";
import ResumeBlock from "@/components/resume/Resume-block";

export default {
  name: 'App',
  components: {
    ResumeBlock,
    MenuBlock,
    SkillsBlock,
    WorksBlock,
    PromoBlock,
    ContactsBlock,
    AboutBlock,
  },
  data() {
    return {
      isMenuOpen: false,
    }
  },
  methods: {
    open() {
      this.isMenuOpen = true;
    },
    close() {
      this.isMenuOpen = false;

    }
  }
}
</script>
