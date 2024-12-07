<script setup>
import NavBar from './components/NavBar.vue';
import Homepage from './components/Homepage.vue';
import AboutUs from './components/AboutUs.vue';
import OurProducts from './components/OurProducts.vue';
import OurExperience from './components/OurExperience.vue';
import ContactUs from './components/ContactUs.vue';
import FrequentlyAsked from './components/FrequentlyAsked.vue';
</script>

<template>
  <NavBar />
   <Homepage />
<div class="wrapper">
   <div class="holder"> 
 <AboutUs />
 <OurProducts />
  </div>
  <OurExperience />
  <ContactUs />
  <FrequentlyAsked />
</div>
</template>

<style scoped>
.wrapper {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.holder {
  width: 90%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: open sans;
}
</style>
