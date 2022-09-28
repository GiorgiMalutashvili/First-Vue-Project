<template>
    <div class="container" id="navigation">
        <div class="row">
            <div class="col-3"><a href="#">Main</a></div>
            <div class="col-3"><a href="#">About</a></div>
            <div class="col-3"><a href="#">Info</a></div>
            <div class="col-3"><a href="#">Contact</a></div>
        </div>
    </div>
</template>

<script>
    export default{
        name: 'MyNavigation',
    }
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@400;500;600;700;800;900&family=Outfit:wght@200;300;400;500&display=swap');

    .container{
        display: grid;
        align-items: center;
        justify-content: end;
    }

    a{
        font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
        text-decoration: none;
        color: #ffffff;
        font-size: 18px;
    }

</style>