<!-- ChildComponentA.vue -->
<template>
  <div>
    <h2>Child Component A</h2>
    <button @click="emitData">Send Data to Parent</button>
  </div>
</template>

<script>
export default {
  methods: {
    emitData() {
      this.$emit('childData', 'Data from Child Component A');
    }
  }
}
</script>

<style scoped>
.child-container {
  text-align: center;
  margin-bottom: 20px;
}

.title {
  color: #007bff;
}

.button {
  background-color: #007bff;
  color: #fff;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.button:hover {
  background-color: #0056b3;
}
</style>