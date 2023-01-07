<template>
  <h3>Hola Mundo estoy haciendo un componente de Nav</h3>
<p>Esta suma da {{(2+2)}}</p>
<h3>Hola {{name}} ¿ves tu nombre en la pantalla? </h3>

</template>




<script setup>

import {ref} from "vue"

const name = ref("Pepe");

/*const name = "Pepe";*/

/*function changeName(){
name.value = "Ramon";

}
*/




</script>




<style>

</style>