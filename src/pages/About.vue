<template>
    <div>
        <Navbar />

           <section class="About">

        <h1 class="heading"> <span>About</span> Me </h1>

        
        <div class="row">

                <div class="w3">

                 <p>Personal Info</p>

                </div>

                <div class="box">
                        <h3> <span>name : </span> Suramesuan Saknitinad </h3>
                        <h3> <span>age : </span> 19 </h3>
                        <h3> <span>email : </span> Suramesuan.sakn@bumail.net </h3>
                        <h3> <span>address : </span> Pathumthani, Thailand 12120 </h3>
                    </div>

                    <div class="box">
                        <h3> <span>Commission : </span> Open </h3>
                        <h3> <span>skill : </span> Photography , Drawing</h3>
                        <h3> <span>experience : </span> 0 years</h3>
                        <h3> <span>language : </span> thai </h3>
                    </div>
                    
                    <br>

                    <div class="box" v-for="e in experiences" :key="e.years">
                        <h3> {{e.years}} </h3>
                        <h3> {{e.schooluni}} </h3>
                    </div>    
                        
            </div>

        </section>

        <!-- skills section starts  -->

        <section class="skills">

            <h1 class="heading"> <span>My</span> Skills </h1>

            <div class="box-container">
                <div class="box">
                    <img src="images/icon-1.png">
                    <h3>Photoshop</h3>
                </div>
                <div class="box">
                    <img src="images/icon-2.png">
                    <h3>Procreate</h3>
                </div>
                <div class="box">
                    <img src="images/icon-3.png">
                    <h3>Photography</h3>
                </div>
                <div class="box">
                    <img src="images/icon-4.png">
                    <h3>Vegas Pro</h3>
                </div>
                <div class="box">
                    <img src="images/icon-5.png">
                    <h3>Maya</h3>
                </div>
                <div class="box">
                    <img src="images/icon-6.png">
                    <h3>Live2d Cubism</h3>
                </div>
            </div>

        </section>

        <!-- skills section ends -->

    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
   export default {
       components: { Navbar },
       data() {
        return {
            experiences: [{
                
            }]
        }
    }
}
</script>

<style>
</style>