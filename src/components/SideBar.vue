<template>
  <div class="container">
    <div class="header">
      <h3>Employees</h3>
    </div>
    <div class="menu">
      <div class="list">
        <span class="text">Directory</span>
      </div>
      <div class="list">
        <span class="text">Update Request</span>
      </div>
      <div class="list">
        <span class="text">Reporting Lines</span>
      </div>
      <div class="list">
        <span class="text">Department structures</span>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  background-color: var(--light-grey);
  min-height: 100vh;
  padding: 1rem;
  align-items: left;
  width: 300px;
}
.container .header {
  margin: 0.4rem 0;
}
.container .menu {
  margin: 0.5rem 0;
}
.container .menu .list {
  display: flex;
  flex-direction: column;
  align-items: left;
  text-decoration: none;
  padding: 1rem 0;
  cursor: pointer;
}
.container .header h3 {
  font-weight: 500;
}
.container .menu .list .text {
  font-weight: 300;
}
.container .menu .list:hover .text,
.container .menu .list:hover {
  color: var(--primary-alt);
}
</style>
