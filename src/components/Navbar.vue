<!-- <script setup>
     import { defineProps} from 'vue';

    defineProps ({
    job: Object
    })
</script> -->
<template>
    <div class="main-container">
        <div class="Nav-container">
            <div class="circle">
               <h2>DTS</h2>
            </div>
            <!-- <p>This Is The Navigation Area</p> -->
             <div class="nav-c">
                <nav class="navbar">
                <ul class="nav-links">
                <li><a href="#" class="nav-item one">Home</a></li>
                <li><a href="#" class="nav-item">Add Schedule</a></li>
                <li><a href="#" class="nav-item">How To Use ?</a></li>
                </ul>
             </nav>
             </div>
        </div>
        <div class="Title-container">
        <h1>Daily Time Schedule</h1> <br><br>
        <h4>Set and Add your new scedule. minimalistic with just our app</h4>
       </div>
    </div>




</template>

<style scoped>

   .main-container {
    background-color: rgb(146, 134, 118);
   }

   .Nav-container {
      background-color: rgb(77, 56, 56);
      top: 0;
      padding: 5px;
      margin: 0;
      height: 15vh;
      /* border: 2px solid rgb(45, 167, 130); */

      /* nested css */
      /* Circle Shape */
            .circle {
            width: 70px; /* Set the width of the circle */
            height: 70px; /* Set the height of the circle */
            background-color:rgb(77, 56, 56); /* Background color */
            border: 2px solid  rgb(146, 134, 118);
            border-radius: 50%; /* Makes the div a circle */
            display: flex; /* Flexbox to center the text */
            align-items: center; /* Vertically center the text */
            justify-content: center; /* Horizontally center the text */
            text-align: center; /* Center text alignment */
            color:  rgb(179, 178, 177); /* Text color */
            }

            .circle h2 {
            margin: 0; /* Remove default margin */
            font-size: 24px; /* Text size */
            font-weight: bold; /* Text weight */
            }

            /* Basic styles for the navigation bar */
            .nav-c {
                position: absolute;
                /* border: 2px solid rgb(199, 18, 18); */
                width: fit-content;
                padding: 0;
                margin: 0;
                top: 5%;
            }
            .navbar {
            /* position: absolute; */
            /* border: 2px solid white; */
            /* background-color: #333; Background color of the navbar */
            padding: 0; /* Padding around the navbar */
            margin-left: 60vw;
            margin-bottom: 2rem;
            width: fit-content;
            }

            .nav-links {
            list-style: none; /* Remove default list styling */
            margin: 0;
            padding: 0;
            display: flex; /* Display links in a row */
            /* justify-content: flex-start; Align links to the left */
            }

            .nav-item {
            color: white; /* Text color */
            text-decoration: none; /* Remove underline from links */
            padding: 0 15px; /* Spacing between links */
            font-size: 18px; /* Font size of links */
        }
        .one {
           background-color: #333;  
        }

            .nav-item:hover {
                background-color: #333;  /* Change color on hover */
            }
   }
   
   .Title-container {
      background-color: rgb(77, 56, 56);
      top: 0;
      padding-top: 30px;
      margin-top: 15px;
      height: 35vh;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: aliceblue;
   }
</style>