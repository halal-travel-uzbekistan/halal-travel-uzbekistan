<template>
    <div class="hello">
        <body>



        <div class="section">

            <h1>Welcome to Uzbekiston</h1>
            <div class="mgs">

                <a href="#test" class="btn btn1">Contact</a>
                <a href="#" class="btn btn2">Explore</a>

            </div>

            <div class="video-container">
                <div class="color-overlay"></div>
                <video id="videoBG" poster="../static/loding.jpg" autoplay muted loop>
                    <source src="../static/uzbekiston.mp4" type="video/mp4">
                </video>
            </div>
        </div>



        <p id="test" style="height: 400px; width: 100%; ">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam aut beatae consectetur deleniti dicta,
            dignissimos doloribus esse in itaque, laudantium mollitia quasi rem saepe sed tempore unde vitae? Sunt,
            voluptatibus?Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium at blanditiis
            consequuntur dicta ducimus eligendi enim eos esse ipsum itaque minus, nemo nesciunt nihil nisi nobis nulla
            quidem temporibus unde. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad atque deserunt fugiat
            laborum repellat veritatis vero voluptatem. Accusantium, adipisci assumenda culpa deserunt eligendi
            inventore maiores natus, ratione sed sequi sunt.</p>


        </body>
    </div>
</template>

<script>
    export default {}
</script>

<style scoped>


    * {
        padding: 0px;
        margin: 0px;
    }


    .section {
        position: relative;
        width: 100%;
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        overflow: hidden;
        flex-direction: column;

    }

    .section h1 {
        text-align: center;
        font-size: 6rem;
        font-family: "Cookie";
        padding: 20px;
        margin: 15px;
        z-index: 1;
        opacity: 0.5;
    }

    .section .mgs{
        z-index: 1;
    }


    .mgs .btn{
        font-size: 18px;
        color: #fff;
        letter-spacing: 2px;
        font-family: "Cookie";
        padding: 7px 28px;
        margin: 5px;
        text-decoration: none;
        border: 1px solid coral;
        border-radius: 25px;
    }

    .btn1{
        background-color: coral;
        color: #fff;

    }

    .btn2:hover{
        background-color: coral;
        transition: .4s;
        border: 2px solid white;
        border-radius: 25px;

    }

    #test{
        transition: 4s all;
    }

    .video-container {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
    }

    .color-overlay {
        position: absolute;
        top: 0;
        left: 0;
        background-color: lightblue;
        width: 100%;
        height: 100vh;
        opacity: 0.5;
    }

</style>
