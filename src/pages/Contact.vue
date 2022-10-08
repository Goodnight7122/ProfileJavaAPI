<template>

    <div>
       <navbar />
       <section class="Contact">
   
        <h1 class="heading">Con<span>tact</span> </h1>

        <div class="Contactcon">

            <form action="">

        <div class="inputBox">
            <input type="text" placeholder="your name">
            <input type="number" placeholder="your number">
        </div>

        <div class="inputBox">
            <input type="email" placeholder="your email">
            <input type="text" placeholder="your subject">
        </div>

        <textarea name="" placeholder="your message" id="" cols="30" rows="10"></textarea>

        <input type="submit" value="send message" class="btn">

    </form>

<div class="box">
    <i class="fas fa-phone"></i>
                <div class="info">
                    <h3>Address:</h3>
                    <p>{{address}}</p>
                    <h3>Email:</h3>
                    <p>{{email}}</p>
                    <h3>Number :</h3>
                    <p>{{number}}</p>

                </div>
</div>


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
            address: 'Pathumthani',
            email: 'suramesuan.sakn@bumail.net',
            number: '+66653242552'
        }
       }
   }
</script>

<style>

</style>