<template>
  <div class="Counter">
    <button @click="++count">Добавить голос {{count}}</button> 
  </div>   
</template>

<script>
import { ref } from 'vue';
export default {
    setup() {
      const count = ref(0);
      return { count };
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  background: blue, 0.5;
  margin: 10px;
  border: 0;
}
</style>
