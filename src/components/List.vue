<template>
  <ol class="output-list">
    <li class="list-item" :key="item" v-for="item in items">{{item}}</li>
  </ol>
</template>

<script>
export default {
  name: "list",
  props: ["items"]
};
</script>

<style scoped>
.output-list {
  list-style: none;
  text-align: center;
}

.list-item {
  margin: 10px;
}

.list-item:hover {
  background: blue;
  color: white;
}
</style>>

  