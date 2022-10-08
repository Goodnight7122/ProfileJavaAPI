<template>
    <div>
       <navbar />
       <section class="Projects">
   
        <h1 class="heading">My<span> Project</span> </h1>
        <p> Project Name: {{project_name}} {{project_detail}}</p>
        <br>
        <br>
        

<div class="content">
    <p style="text-align: center;"><iframe width="1280" height="720" src="https://www.youtube.com/embed/bnmAi53H520" title="Noot Noot" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>
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
            project_name: 'Noot Noot',
            project_detail: 'Pain',
        }
       }
   }

</script>

<style>

</style>