<template>
  <div :class="{hidden:!show, container:true}">
    <h1 class="title">PROFILE</h1>
  </div>
</template>

<script>
export default {
  name: 'ProfileView',
  props:{
    show:Boolean
  }
}
</script>

<style>
.hidden{
  display: none;
}
</style>