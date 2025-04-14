<template>
 <div v-show="isVisible">i m visible</div>
 <div>Visibility: {{ isVisible }}</div>
</template>

<script>

export default {
data() {
return {
isVisible: true
}
}}
</script>

<style scoped>
* {
  margin: 0 0 0 10px;
  padding: 10px;
}
</style>
