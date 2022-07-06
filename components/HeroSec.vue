<template>
    <div class="w-full h-screen font-pop text-white">
        <header class="container flex justify-between items-center pt-12 mx-auto">

            <a href="#" class="logo text-2xl font-black pr-96">Morgan.<span>Agee</span></a>

            <nav class="space-x-12 pl-96 border-r-4 border-dotted">
                <a href="#">My Story</a>
                <a href="#">Journal</a>
                <a href="#" class="pr-16">Contact</a>
            </nav>

            <div class='flex justify-between space-x-5'>
                <a target='_blank' href='https://instagram.com/alexamorgannn?igshid=YmMyMTA2M2Y='><img src="../static/Insta.png" alt="Instagram" class='w-11 h-11' ></a>
                <a target='_blank' href="https://www.linkedin.com/in/alexandra-morgan-agee-548579112"><img src="../static/linkedin.png" alt="Linkedin" class='w-11 h-11'></a>
            </div>
        </header>

        <section class="flex flex-col justify-center items-center w-full h-screen">
        
            <h1 class="text-9xl text-center mb-10">Lorem ipsum dolor<br>sit amet consectetur.</h1>
        
            <a target='_blank' href='https://www.linkedin.com/messaging/thread/new/?recipients=List(urn%3Ali%3Afsd_profile%3AACoAABw0UsgBIpoW1IhXSkeO4-wdDvdFryLvA5g)&composeOptionType=CONNECTION_MESSAGE&controlUrn=sticky_header_primary_compose_message_button&referringModuleKey=NON_SELF_PROFILE_VIEW&messageComposeFlowTrackingId=fIgJ246pR0mCCYvTtJi0hA%3D%3D'><button class="p-4 bg-blue-700 text-4xl rounded-2xl">Hire Me</button></a>

        </section>
    </div>
</template>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;800&display=swap');

    span {
        color: blue;
    }

    body {
        background-image: url('../static/plant2.jpg');
        margin: 0 auto;
    }
    button:hover {
        background-color: #fff;
        color: blue;
    }
    a:hover {
        color: blue;
    }
</style>