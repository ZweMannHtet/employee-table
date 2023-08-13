<template>
  <div class="app">
    <ActiveBar />
    <SideBar />
    <Body />
  </div>
</template>

<script setup>
import ActiveBar from "./components/ActiveBar.vue";
import SideBar from "./components/SideBar.vue";
import Body from "./Category/Body.vue";
</script>

<style>
:root {
  --primary: #62d08a;
  --primary-alt: #22c55e;
  --grey: #64748b;
  --light-grey: #d3d3d3;
  --dark: #1e293b;
  --dark-alt: #334155;
  --light: #f1f5f9;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}

body {
  background: var(--light);
}

.app {
  display: flex;
  min-height: 100vh;
}

@media (max-width: 1024px) {
  .app main {
    padding-left: 6rem;
  }
}
</style>
