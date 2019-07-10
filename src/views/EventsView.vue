<template>
  <div :class="{hidden:!show, container:true}">
    <h1 class="title">EVENTS</h1>
  </div>
</template>

<script>
export default {
  name: 'EventsView',
  props:{
    show:Boolean
  }
}
</script>

<style scoped>
.hidden{
  display: none;
}
</style>