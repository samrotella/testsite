<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button v-on:click="conversion()">Buy Now</button>
  </div>
</template>

<script>
// import owlsight from "https://owlsight.onrender.com/main.js";

export default {
  name: "About",
  data() {
    return {
    };
  },
  methods: {
    conversion() {
      owlsight.conversions('SKU-123', 42.22);
    },
  },
};
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
