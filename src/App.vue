<template>
  <promo-block/>
  <about-block/>
  <contacts-block/>
</template>

<script>

import AboutBlock from "./components/about/About-block";
import ContactsBlock from "@/components/contacts/Contacts-block";
import PromoBlock from "@/components/promo/Promo-block";

export default {
  name: 'App',
  components: {
    PromoBlock,
    ContactsBlock,
    AboutBlock,
  }
}
</script>
