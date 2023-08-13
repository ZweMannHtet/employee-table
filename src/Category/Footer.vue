<template>
  <div class="container">
    <div class="flex"></div>
    <div class="bottom">
      <div class="select">
        <select>
          <option value="">50/page</option>
        </select>
      </div>
      <div class="paginate">
        <span class="previous">&lt;</span>
        <span class="one">1</span>
        <span>2</span>
        <span>3</span>
        <span class="next">></span>
      </div>
      <div class="page">
        <p>Go to</p>
        <span class="pageOne">1</span>
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
  justify-content: space-between;
  position: sticky;
  bottom: 0;
}
.bottom {
  display: flex;
  align-items: center;
  text-decoration: none;
  cursor: pointer;
  margin: 0;
}
p {
  margin-right: 10px;
}

.one {
  background-color: var(--primary);
  color: var(--light);
}
.page {
  display: flex;
  align-items: center;
  padding: 0.75rem;
  margin: 0 5px;
}
.pageOne {
  display: inline-block;
  text-align: center;
  padding: 10px;
  border: 1px solid rgb(166, 158, 158);
  width: 50px;
  height: 40px;
  border-radius: 5px;
}

select {
  padding: 10px;
  margin: 0 30px;
}
.paginate {
  margin: 0 30px;
  border-radius: 10px;
}

.paginate span {
  display: inline-block;
  text-align: center;
  padding: 10px;
  border: 1px solid rgb(166, 158, 158);
  width: 40px;
  height: 40px;
}
</style>
