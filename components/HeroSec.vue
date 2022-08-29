<template>
    <div class="w-full h-screen font-pop text-white overflow-hidden">
        <header class="container flex justify-between items-center pt-12 mx-auto">

            <div class="logo text-2xl font-black pr-96" @click="showModal = true">Morgan.<span>Agee</span></div>
            <!-- MY FIRST MODAL POP-UP -->
            <transition name="fade" appear>
                <div v-if="showModal" class="modal-overlay"  @click="showModal = false"></div>
            </transition>
            <transition name="slide" appear>
                <div  v-if="showModal" class="modal">
                    <img src="../static/Morgan's Resume.png">
                    <button class="button" @click="showModal = false">
                        Close Modal
                    </button>
                </div>
            </transition>
            
            <nav class="space-x-12 pl-96 border-r-4 border-dotted" >
                <a target='_blank' href="https://www.linkedin.com/in/alexandra-morgan-agee-548579112/details/experience/">Work History</a>
                <a href="#">Achievements</a>
                <a href="#" class="pr-16">Contact</a>
            </nav>

            <div class='flex justify-between space-x-5'>
                <a target='_blank' href='https://instagram.com/alexamorgannn?igshid=YmMyMTA2M2Y='><img src="../static/Insta.png" alt="Instagram" class='w-11 h-11' ></a>
                <a target='_blank' href="https://www.linkedin.com/in/alexandra-morgan-agee-548579112"><img src="../static/linkedin.png" alt="Linkedin" class='w-11 h-11'></a>
            </div>
        </header>

        <section class="flex flex-col items-center w-full h-screen pt-96 mt-10">
        
            <h1 class="text-9xl text-center mb-10">Lorem ipsum dolor<br>sit amet consectetur.</h1>
        
            <a target='_blank' href='https://www.linkedin.com/messaging/thread/new/?recipients=List(urn%3Ali%3Afsd_profile%3AACoAABw0UsgBIpoW1IhXSkeO4-wdDvdFryLvA5g)&composeOptionType=CONNECTION_MESSAGE&controlUrn=sticky_header_primary_compose_message_button&referringModuleKey=NON_SELF_PROFILE_VIEW&messageComposeFlowTrackingId=fIgJ246pR0mCCYvTtJi0hA%3D%3D'><button onclick="reveal" class="p-4 bg-blue-700 text-4xl rounded-2xl">Hire Me</button></a>

        </section>
    </div>
</template>

<script>
    export default {
        data: function () {
            return {
                showModal: false
            }
        }
    }
</script>

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

::-webkit-scrollbar {
    display: none;
}

.logo {
    cursor: pointer;
}

.logo:hover {
    text-shadow:black 0px 0px 10px;
}

/*Modal*/

.modal-overlay {
 position: absolute;
 top: 0;
 left: 0;
 right: 0;
 bottom: 0;
 z-index: 98;
 background-color: rgba(0, 0, 0, 0.3);
}

.modal {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 99;
 
    width: 100%;
    max-width: 900px;
    background-color: #FFF;
    border-radius: 16px;
 
    padding: 25px;
}

.fade-enter-active,
.fade-leave-active {
    transition: opacity .5s;
}

.fade-enter,
.fade-leave-to {
    opacity: 0;
}

.slide-enter-active,
.slide-leave-active {
    transition: transform .5s;
}

.slide-enter,
.slide-leave-to {
    transform: translateY(-50%) translateX(100vw);
}
</style>
