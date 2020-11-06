<template>
  <teleport to="#modal">
    <div id="center">
      <h1>this is a modal</h1>
    </div>
  </teleport>
</template>

<script>
export default {
  name: 'model'
}
</script>

<style scoped >
#center {
  width: 200px;
  height: 200px;
  background: red;
  position: fixed;
  left: 50%;
  top: 50%;
  margin-left: -100px;
  margin-top: -100px;
}
</style>
