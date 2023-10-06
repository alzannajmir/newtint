<script setup>
import NavbarVue from "./components/Navbar.vue";
import HeroVue from "./components/Hero.vue";
import PurchaseVue from "./components/Purchase.vue";
import FooterVue from "./components/Footer.vue";
import AdvantageVue from "./components/Advantage.vue";

</script>

<template>
  <div>
    <section id="Navbar">
      <NavbarVue />
    </section>

    <section id="Hero">
      <HeroVue />
    </section>

    <section id="Advantage">
      <advantageVue />
    </section>

    <section id="Purchase">
      <PurchaseVue />
    </section>
    
       <section id="Footer">
      <FooterVue />
  </div>
</template>
