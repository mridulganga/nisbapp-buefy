<template>
  <div id="app">
    <home-view :show="'HOME'==currentView"/>
    <events-view :show="'EVENTS'==currentView"/>
    <announcements-view :show="'ANNOUNCEMENTS'==currentView"/>
    <profile-view :show="'PROFILE'==currentView"/>

    <nav-bar
      @view-changed="changeView"/>
  </div>
</template>

<script>
import Vue from 'vue'
import Buefy from 'buefy'
import 'buefy/dist/buefy.css'

Vue.use(Buefy)

import HomeView from './views/HomeView.vue'
import EventsView from './views/EventsView.vue'
import AnnouncementsView from './views/AnnouncementsView.vue'
import ProfileView from './views/ProfileView.vue'

import NavBar from './components/NavBar.vue'

export default {
  name: 'app',
  data(){
    return{
      currentView: "HOME"
    }
  },
  components: {
    HomeView,EventsView,AnnouncementsView,ProfileView,
    NavBar
  },
  methods:{
    changeView(v){
        this.currentView = v
    }
  },
  
}
</script>

<style>

.container{
  padding: 60px 20px;
}

.title{
  padding: 20px 10px;
}

.hidden{
  display: none;
}
</style>
