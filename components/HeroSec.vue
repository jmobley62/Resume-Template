<template>
    <div class="w-full h-screen font-pop text-white">
        <header class="container flex justify-between items-center pt-12 mx-auto">

            <div id="myImg" class="logo text-2xl font-black pr-96" >Morgan.<span>Agee</span></div>
            <img id="theImg" src="../static/snow.jpg" alt="" >

            <!-- The Modal -->
            <div id="myModal" class="modal">
                <span class="close">&times;</span>
                <img id="img01" class="modal-content" >
            </div>

            <nav class="space-x-12 pl-96 border-r-4 border-dotted">
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
// Get the modal
const modal = document.getElementById("myModal");

// Get the image and insert it inside the modal - use its "alt" text as a caption
const img = document.getElementById("myImg");
const modalImg = document.getElementById("img01");
const theImg = document.getElementById("theImg");
img.onclick = function(){
  modal.style.display = "block";
  modalImg.src = theImg.src;
}

// Get the <span> element that closes the modal
const span = document.getElementsByClassName("close")[0];

// When the user clicks on <span> (x), close the modal
span.onclick = function() { 
  modal.style.display = "none";
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

/*Modal*/

#myImg {
  border-radius: 5px;
  cursor: pointer;
  transition: 0.3s;
}

#myImg:hover {opacity: 0.7;}

/* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  padding-top: 100px; /* Location of the box */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: rgb(0,0,0); /* Fallback color */
  background-color: rgba(0,0,0,0.9); /* Black w/ opacity */
}

/* Modal Content (image) */
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

/* Caption of Modal Image */
#caption {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  text-align: center;
  color: #ccc;
  padding: 10px 0;
  height: 150px;
}

/* Add Animation */
.modal-content, #caption {  
  -webkit-animation-name: zoom;
  -webkit-animation-duration: 0.6s;
  animation-name: zoom;
  animation-duration: 0.6s;
}

@-webkit-keyframes zoom {
  from {-webkit-transform:scale(0)} 
  to {-webkit-transform:scale(1)}
}

@keyframes zoom {
  from {transform:scale(0)} 
  to {transform:scale(1)}
}

/* The Close Button */
.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}

/* 100% Image Width on Smaller Screens */
@media only screen and (max-width: 700px){
  .modal-content {
    width: 100%;
  }
}

#theImg {
    display:none;
}
</style>