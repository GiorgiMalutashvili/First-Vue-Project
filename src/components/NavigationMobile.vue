<template>
    <div class="container-fluid" id="navigation-mobile">
        <div class="row">
            <div class="col"><a href="#">Main</a></div>
            <div class="col"><a href="#">About</a></div>
            <div class="col"><a href="#">Info</a></div>
            <div class="col"><a href="#">Contact</a></div>
            <div class="col"><a href="#">Author</a></div>
        </div>
        <div class="social-media">
            <i class="fab fa-twitter"></i>
            <i class="fab fa-instagram"></i>
            <i class="fab fa-facebook"></i>
        </div>
    </div>
</template>

<script>
    export default{
        name: 'NavigationMobile',
    }
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@400;500;600;700;800;900&family=Outfit:wght@200;300;400;500&display=swap');

    .container-fluid{

        display: grid;
        align-items: center;
        justify-content: start;
    }

    .row{
        display: flex;
        flex-direction: column;
        gap: 20px;
        margin-top: 30px;
    }

    a{
        font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        text-decoration: none;
        color: #ffffff;
        font-weight: bold;
        font-size: 18px;
        padding: 2px 10px;
    }
    a:hover{
        color: blueviolet;
    }
    #navigation-mobile{
        padding: 25px 10 0 0 ;
    }
    .col{
        width: 210px;
        padding-left: 0;
    }
    .social-media{
        display: flex;
        gap: 20px;
        position: absolute;
        bottom: 20px;
    }
    i{
        color: #ffffff;
    }
    i:hover{
        color: blueviolet;
    }

</style>