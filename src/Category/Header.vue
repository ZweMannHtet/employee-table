<template>
  <div class="container">
    <div class="first-box">
      <div class="icon text-icon">
        <span class="material-icons">west</span>
        <span class="text">Employee Directory</span>
      </div>
      <div class="icon">
        <span class="material-icons">filter_alt</span>
      </div>
      <div class="icon">
        <span class="material-icons">search</span>
      </div>
      <div class="icon icon-pen">
        <span class="material-icons">edit</span>
      </div>
    </div>

    <div class="end-box">
      <div class="button">
        <button>Create Employee</button>
      </div>
      <div class="icon">
        <span class="material-icons">more_vert</span>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.parent {
  width: 100%;
}
.container {
  display: flex;
  background-color: var(--light);
  padding: 0.5rem;
  align-items: center;
  margin: 0;
  border-bottom: 1px solid rgb(220, 208, 208);
  justify-content: space-between;
  width: 100%;
  position: sticky;
  top: 0;
}
.first-box {
  display: flex;
  align-items: center;
  text-decoration: none;
  cursor: pointer;
  margin: 0;
}

.end-box {
  display: flex;
  align-items: center;
}
.icon {
  display: flex;
  align-items: center;
  padding: 0.75rem;
  margin: 0 5px;
}
.icon-pen {
  max-height: 30px;
  padding-left: 15px;
  /* overflow: hidden; */
  border-left: 1px solid rgb(220, 200, 200);
}
.material-icons {
  font-size: 35px;
}
.text-icon .material-icons {
  color: var(--primary-alt);
}
.text {
  margin-left: 0.5rem;
  font-weight: 400;
  font-size: 1.1rem;
}
button {
  padding: 15px;
  background-color: var(--primary);
  color: white;
  border-radius: 5px;
}
</style>
