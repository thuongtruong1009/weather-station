<template>
  <div class="container">
    <Box />
    <Table />
  </div>
</template>

<script>
import Box from "./components/Box.vue";
import Table from "./components/Table.vue";
export default {
  name: "App",
  components: {
    Box,
    Table,
  },
};
</script>
<style>
.container {
  background: rgba(0, 43, 0, 0.541);
  display: grid;
  justify-content: center;
  align-items: center;
  height: 99vh;
}
</style>

