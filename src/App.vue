<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/pp.jpg" width="300" height="400" />

    <div class="wrapper">
      <HelloWorld msg="Welcome To My Profile!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  animation: slideUpDown 5s infinite alternate; /* Menggunakan animasi slideUpDown selama 5 detik dan diulang-ulang */
}

@keyframes slideUpDown {
  0% {
    transform: translateY(0); /* Mulai dari posisi awal */
  }
  100% {
    transform: translateY(100px); /* Bergerak ke bawah sejauh 100px */
  }
}

</style>
