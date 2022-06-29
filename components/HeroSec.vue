<template>
    <div class="w-full h-screen font-pop text-white">
        <header class="container flex justify-between items-center pt-12 mx-auto">

            <a href="#" class="logo text-2xl font-black pr-96">Morgan.<span>Agee</span></a>

            <nav class="space-x-12 pl-96">
                <a href="#">My Story</a>
                <a href="#">Journal</a>
                <a href="#">Contact</a>
            </nav>

            <div class="bg-black">
                <a href="">IG</a>
                <a href="">TWITTER</a>
            </div>
        </header>

        <section class="flex flex-col justify-center items-center w-full h-screen">
        
            <h1 class="text-9xl text-center mb-10">Lorem ipsum dolor<br>sit amet consectetur.</h1>
        
            <button class="p-4 bg-blue-700 text-4xl rounded-2xl">Hire Me</button>

        </section>
    </div>
</template>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;800&display=swap');

    span {
        color: red;
    }

    body {
        background-image: url('../static/plant2.jpg');
        margin: 0;
    }
    button:hover {
        background-color: #fff;
        color: blue;
    }
</style>