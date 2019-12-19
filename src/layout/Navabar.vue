<template>
 <div>

     <div class="nav">
         <img src="../static/logo1.png" class="logo">
         <ul class="menu">
             <li><a href="#">Home</a></li>
             <li><a href="#">About</a></li>
             <li><a href="#">Service</a></li>
             <li><a href="#">Revies</a></li>
             <li><a href="#">Contact</a></li>
         </ul>


     </div>


 </div>
</template>

<script>
    export default {
    }
</script>

<style scoped>


    .nav{
        background: rgb(0,0,0,.5);
        height: 80px;
    }

    .logo{
        margin: 10px 50px;
        height: 60px;
    }

    .menu{
        float: right;
        list-style: none;
        margin: 20px;
    }

    .menu li{
        display: inline-block;
        margin: 10px 5px;
    }

    .menu a{
        text-decoration: none;
        color: #fff;
        padding: 5px 10px;
        font-family: "Cookie";
        letter-spacing: 2px;
        border-bottom: 1px solid #fff;

    }


    .menu li a:hover{
        background: coral;
        border-bottom: 1px solid coral;
        transition: .4s;

    }




</style>