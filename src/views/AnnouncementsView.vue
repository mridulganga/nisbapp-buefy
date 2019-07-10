<template>
  <div :class="{hidden:!show, container:true}">
    <h1 class="title">ANNOUNCEMENTS</h1>
  </div>
</template>

<script>
export default {
  name: 'AnnouncementsView',
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