<!-- ParentComponent.vue -->
<template>
  <div>
    <h1>Parent Component</h1>
    <ChildComponentA @childData="handleChildData" />
    <ChildComponentB :receivedData="receivedData" />
  </div>
</template>

<script>
import ChildComponentA from './components/ChildComponentA.vue'
import ChildComponentB from './components/ChildComponentB.vue'

export default {
  components: {
    ChildComponentA,
    ChildComponentB
  },
  data() {
    return {
      receivedData: ''
    }
  },
  methods: {
    handleChildData(data) {
      this.receivedData = data;
    }
  }
}
</script>

<style scoped>
.parent-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  background-color: #f9f9f9;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.title {
  color: #333;
  text-align: center;
  margin-bottom: 20px;
}

</style>