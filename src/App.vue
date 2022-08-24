<template>
  <div class="app">
    App.vue 我现在有 {{total}}
    <hr>
    <Child :money.sync="total"/>
  </div>
</template>

<script>
import Child from "./Child.vue";
export default {
  data() {
    return { total: 10000 };
  },
  components: { Child: Child }
};
</script>

<style>
.app {
  border: 3px solid red;
  padding: 10px;
}
</style>
