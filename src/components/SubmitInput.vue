<template>
  <form class="input-form" @submit.prevent="addItem">
    <input v-model="newItem" type="text" />
    <button type="submit">Submit</button>
  </form>
</template>

<script>
export default {
  name: "SubmitInput",
  data() {
    return {
      newItem: ""
    };
  },
  methods: {
    addItem(event) {
      this.$emit("new-item", this.newItem);
      console.log(this.newItem);
      this.newItem = "";
    }
  }
};
</script>

<style scoped>
</style>>

