<script setup>
import { ref } from 'vue'

const num = ref(2)
function clickMe() {
  num.value++
}
</script>

<template>
  <div class="abcc">
    <div>hello ^^ v</div>
    <p>&nbsp;{{ num }}&nbsp;</p>
    <button type="button" v-on:click="clickMe">CLICK</button>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}
.abcc {
  display: flex;
  justify-content: center;
  align-items: center;
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
</style>
