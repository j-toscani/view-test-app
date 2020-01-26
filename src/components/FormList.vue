<template>
  <div class="container">
    <submitInput @new-item="addNewItemToList"></submitInput>

    <list :items="items"></list>
  </div>
</template>

<script>
import List from "./List";
import SubmitInput from "./SubmitInput";

export default {
  name: "FormList",
  components: {
    list: List,
    submitInput: SubmitInput
  },
  data() {
    return {
      newItem: "",
      items: ["Banana", "Apple", "Potato"]
    };
  },
  methods: {
    addNewItemToList(value) {
      console.log(value);
      this.items.push(value);
    }
  }
};
</script>

<style scoped>
div.container {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.output-list {
  list-style: none;
  text-align: center;
}

.new_item,
.list-item {
  margin: 10px;
}

.list-item:hover {
  background: blue;
  color: white;
}
</style>>

