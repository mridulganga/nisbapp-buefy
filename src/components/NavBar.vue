<template>
    <section class="fixed-bottom box">
        <b-button @click="homeClick" type="is-light" class="one-four"><i class="fas fa-home"></i></b-button>
        <b-button @click="eventsClick" type="is-light" class="one-four"><i class="fas fa-calendar-check"></i></b-button>
        <b-button @click="announcementsClick" type="is-light" class="one-four"><i class="fas fa-bell"></i></b-button>
        <b-button @click="profileClick" type="is-light" class="one-four"><i class="fas fa-user"></i></b-button>

    </section>
</template>

<script>
export default {
    name: "NavBar",
    methods:{
        homeClick(){
            this.$emit("view-changed","HOME");
        },
        eventsClick(){
            this.$emit("view-changed","EVENTS");
        },
        announcementsClick(){
            this.$emit("view-changed","ANNOUNCEMENTS");
        },
        profileClick(){
            this.$emit("view-changed","PROFILE");
        }        
    }
}
</script>

<style scoped>
.one-four{
    width:25%;
    border: 0;
    font-size: 1.3em;
    border-radius: 0;
}
.one-four:hover{
    border: 0;
}
.one-four:active{
    border: 0;
}
.fixed-bottom{
    position: fixed;
    bottom: 0;
    width: 100%;
    left: 0;
}
.box{
    padding: 0;
}
</style>
