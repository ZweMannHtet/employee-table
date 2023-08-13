<template>
  <div class="container">
    <div>
      <div class="logo">
        <img :src="logo" alt="logo" />
      </div>

      <div class="menu">
        <div class="icon">
          <span class="material-icons">desktop_windows</span>
        </div>
        <div class="icon">
          <span class="material-icons">schedule</span>
        </div>
        <div class="icon">
          <span class="material-icons">business_center</span>
        </div>
        <div class="icon">
          <span class="material-icons">more_time</span>
        </div>
        <div class="icon">
          <span class="material-icons">person</span>
        </div>
        <div class="icon">
          <span class="material-icons">autorenew</span>
        </div>
        <div class="icon">
          <span class="material-icons">notifications</span>
        </div>
        <div class="icon">
          <span class="material-icons">credit_card</span>
        </div>
        <div class="icon">
          <span class="material-icons">sms</span>
        </div>
        <div class="icon">
          <span class="material-icons">more_horiz</span>
          <span class="text">more</span>
        </div>
      </div>
    </div>

    <div>
      <div class="menu">
        <div class="icon">
          <span class="material-icons">note</span>
        </div>
        <div class="icon">
          <span class="material-icons">mark_chat_unread</span>
        </div>
        <div class="image">
          <img src="../user/2.jpeg" alt="profile" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import logo from "../assets/logo.png";
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  background-color: var(--dark);
  padding: 1rem;
  align-items: center;
  justify-content: space-between;
}
.text {
  color: wheat;
}

.logo {
  margin-bottom: 1rem;
}

.logo img {
  width: 2rem;
}

.menu {
  margin: 0 -1rem;
  align-items: center;
}

.icon {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-decoration: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
}

.material-icons {
  font-size: 2rem;
  color: var(--light);
  transition: 0.2s ease-in-out;
}

.icon:hover {
  background-color: var(--light-grey);
}
.image img {
  border-radius: 50%;
  width: 3rem;
  margin-left: 9px;
}

.icon:hover .material-icons,
.icon:hover {
  color: var(--primary-alt);
}
@media (max-width: 1024px) {
  .container {
    z-index: 99;
  }
}
</style>
