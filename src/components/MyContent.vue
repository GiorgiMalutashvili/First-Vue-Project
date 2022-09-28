<template>
    <div class="container">
        <div class="row">
            <div class="col-sm-6"><img src="../assets/explore.jpg" alt=""></div>
            <div class="col-sm-6"><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus nemo nam quo impedit a blanditiis, maxime consequatur eius, atque tempora illum qui. Voluptatibus, sapiente voluptatem et laboriosam in quos enim.   </p>
            </div>
          </div>
    </div>
   
</template>

<script>
    export default{
        name: 'MyCOntent',
    }
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@400;500;600;700;800;900&family=Outfit:wght@200;300;400;500&display=swap');

    .container{
        display: flex;
        flex-direction: column;
        width: 97%;
        margin-top: 10%;
    }

    img{
        width: 100%;
        height: 50vh;
        border-radius: 10px;
    }
    p{
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        font-weight: 300;
        font-size: 16px;
    }
</style>