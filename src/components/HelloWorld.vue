<template>
  <div>{{msg}}</div>
</template>

<script>
export default {
  props: ["msg"]
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.box {
  height: 60px;
  width: 60px;
  background: red;
}
</style>
