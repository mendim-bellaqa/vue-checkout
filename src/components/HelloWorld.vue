<script>
export default {
  data() {
    return {
      name: '',
      surename: '',
      card_number: '',
      expiry_date: '',
      cvc: '',
      cvv: '',


    }
  }
}
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      <p>Your name: {{ name }}</p>
      <p>Your surename: {{ surename }}</p>
      <p>Your card number: {{ card_number }}</p>
      <p>Your expiry date: {{ expiry_date }}</p>
      <p>Your cvc: {{ cvc }}</p>
      <p>Your cvv: {{ cvv }}</p>
      
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>.
    </h3>
    <input v-model="name" placeholder="Enter your name" class="card-imput"/>
    <input v-model="surename" placeholder="Enter your suername" class="card-imput" />
    <input v-model="card_number" placeholder="Enter your card numbers" class="card-imput" />
    <input v-model="expiry_date" placeholder="Enter  your card's expity date" class="card-imput" />
    <input v-model="cvc" placeholder="Enter your CVC" class="card-imput" />
    <input v-model="cvv" placeholder="Enter your CVV" class="card-imput"/>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.card-imput{
  margin-top: 15px;
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
