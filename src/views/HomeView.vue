<template>
  <div :class="{hidden:!show, container:true}">
    <h1 class="title">NISB</h1>

    <h2 class="subtitle">Upcoming Events</h2>

    <div class="horizontal-scroll">
      <img src="https://www.dropbox.com/s/bb4m4hojb8vhhol/R%20Pi%20%281%29.png?raw=1" class="fix-height">
      <img src="https://www.dropbox.com/s/n6xz8vtqiivlzbz/SelfHosted%20%281%29.png?raw=1" class="fix-height">
      <img src="https://www.dropbox.com/s/bb4m4hojb8vhhol/R%20Pi%20%281%29.png?raw=1" class="fix-height">
    </div><br><br>
    
    <h2 class="subtitle">Latest Announcements</h2>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  props:{
    show:Boolean
  }
}
</script>

<style scoped>
.horizontal-scroll{
  overflow-x: scroll;
  overflow-y: hidden;
  height: 150px;
  white-space:nowrap

}

.fix-height{
  height: 150px;
  margin-left: 10px;
}
</style>
