<script setup lang="ts">
import Navbar from './components/Navbar.vue';
import ScrollReveal from './components/ScrollReveal.vue';
import Customize from './sections/Customize.vue';
import Hero from './sections/Hero.vue';
import Plan from './sections/Plan.vue';
import WorkManagement from './sections/WorkManagement.vue';

</script>


<template>
    <Navbar />
  
    <section id="hero" class="pt-[92px]">
  <ScrollReveal enterClass="opacity-100 translate-y-0" exitClass="opacity-0 translate-y-10">
    <Hero />
  </ScrollReveal>
</section>

  
    <section id="work">
      <ScrollReveal enterClass="opacity-100 translate-x-0" exitClass="opacity-0 -translate-x-10">
        <WorkManagement />
      </ScrollReveal>
    </section>
  
    <section id="customize">
      <ScrollReveal enterClass="opacity-100 scale-100" exitClass="opacity-0 scale-95">
        <Customize />
      </ScrollReveal>
    </section>
  
    <section id="plan">
      <ScrollReveal enterClass="opacity-100 translate-y-0" exitClass="opacity-0 translate-y-10">
        <Plan />
      </ScrollReveal>
    </section>
  </template>
  

