<template>
  <NavbarVue/>

  <p v-bind:class="show"> Este texto es condicional</p>
  <button @click="changeColor">Change Color</button>
  <FooterVue/>
</template>

<script setup>
import NavbarVue from './components/Navbar.vue';
import FooterVue from './components/Footer.vue';
import { ref } from 'vue';

const show = ref("show");

function changeColor(){
  show.value="hidden";
}


</script>

<style scoped>



.show{
background-color:white;

}

.hidden{
  background-color: red;
}
.logo {

  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
