{/*export default { //data() { return { count: 0, }; }, methods: { increment() {
this.count++; }, decrement() { this.count--; }, }, }; */}
<script setup>
import { ref } from "vue";
const count = ref(5);
const increment = () => {
  count.value++;
};
const decrement = () => {
  count.value--;
};
</script>

<template>
  <div>
    <h2>count is {{ count }}</h2>
    <button @click="increment">Inc</button>
    <button @click="decrement">Dec</button>
  </div>
</template>
