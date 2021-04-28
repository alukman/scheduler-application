<template>
   <div>
      <b-jumbotron>
         <template #header> Scheduler </template>
         <template #lead> Login to continue </template>
         <hr />
         <login />
      </b-jumbotron>
   </div>
</template>

<script>
import Login from "./Login.vue";
export default {
   components: {
      Login,
   },
};
</script>

