<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  
  <header>
    <img alt="Card" class="logo" src="./assets/payment-card.png" width="780" height="450" />

    <div class="wrapper">
      <HelloWorld msg="Checkout form !" />
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
  position: relative;
  margin-left:-120px;
  margin-top: -120px;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    position: relative;
    margin-left:-180px;
    margin-top: -10px;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
