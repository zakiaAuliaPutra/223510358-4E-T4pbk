<!-- ChildComponentB.vue -->
<template>
  <div>
    <h2>Child Component B</h2>
    <p>Data Received from Parent: {{ receivedData }}</p>
  </div>
</template>

<script>
export default {
  props: ['receivedData']
}
</script>

<style scoped>
.child-container {
  text-align: center;
}

.title {
  color: #28a745;
}

.data {
  font-size: 16px;
  margin-top: 10px;
}
</style>