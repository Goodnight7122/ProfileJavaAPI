<template>
 <div>
    <navbar />
    <section class="home">

<div class="image">
    <img src="images/profile.png" alt="">
</div>

<div class="content">
    <h3>Hi am {{name}}</h3>
    <span>"{{motto}}"</span>
    <p>{{content}}</p>
    <a href="About" class="btn"> about me <i class="fas fa-user"></i> </a>
</div>

</section>
 </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar },
    data() {
        return {
            name: 'Suramesuan Saknitinad',
            motto: 'Learning By Doing',
            content: 'Hi am Good I am now studying at Multimedia and Entertainment Engineering Bangkok University and This is my profile.'
        }
    }
}
</script>

<style>

</style>