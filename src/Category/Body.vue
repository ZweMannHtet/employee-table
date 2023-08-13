<template>
  <div class="box">
    <Header />
    <Employee />
    <Footer />
  </div>
</template>

<script setup>
import Header from "./Header.vue";
import Footer from "./Footer.vue";
import Employee from "./Employee.vue";
</script>

<style scoped>
.box {
  width: 80%;
  margin: 0 0 0 40px;
}
</style>
