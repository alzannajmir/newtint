<script setup>
import NavbarVue from "./components/Navbar.vue";
import HeroVue from "./components/Hero.vue";
import PurchaseVue from "./components/Purchase.vue";
import AdvantageVue from "./components/Advantage.vue";
import Information from "./components/Information.vue";
import Product from "./components/Products.vue";
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
      <AdvantageVue />
    </section>

    <section id="Product">
      <Product />
    </section>

    <section id="Information">
      <Information />
    </section>


    <section id="Purchase">
      <PurchaseVue />
    </section>
  </div>
</template>

