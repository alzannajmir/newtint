<script setup>
import NavbarVue from "./components/Navbar.vue";
import HeroVue from "./components/Hero.vue";
import PurchaseVue from "./component/Purchase.vue";
</script>

<template>
  <div>
    <section id="Navbar">
      <NavbarVue />
    </section>

    <section id="Hero">
      <HeroVue />
    </section>

    <section id="Purchase">
      <PurchaseVue />
    </section>
  </div>
</template>
