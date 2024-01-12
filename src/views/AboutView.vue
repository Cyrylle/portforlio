<script setup>
import MainLayout from '../components/MainLayout.vue';

// Page Title of Views
const pageTitle = 'About'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">
    <section>
      <div class="w-full bg-amber-800">
    <section class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-4 py-12">
        <div class="text-center pb-12">
            <h1 class="font-bold text-3xl md:text-4xl lg:text-5xl font-heading text-black font-serif">
                ABOUT ME
            </h1>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
            <div class="w-full bg-gray-900 rounded-lg sahdow-lg overflow-hidden flex flex-col md:flex-row">
                <div class="w-full  h-80">
                    <img class="object-center object-cover w-full h-full" src="../assets/wq.jpg" alt="gabo">
                </div>
                <div class="w-full md:w-3/5 text-left p-6 md:p-4 space-y-2">
                    <p class="text-xl text-white font-bold">PERSONAL INFORMATION</p>
                  
                    <p class="text-base leading-relaxed text-gray-500 font-normal">Hi, I am Cyrylle Nate Sanchez. 22 years old. I lived in Buagsong, Cordova, Cebu. </p>
                </div>
            </div>
            <div class="w-full bg-gray-900 rounded-lg sahdow-lg  flex flex-col md:flex-row">
                <div class=" p-4 md:p-4 space-y-2">
                  <p class="text-xl text-white font-bold">HOBBIES</p>
                    <p class="text-base leading-relaxed text-justify text-gray-500 font-normal">As an IT student, Passionate about technology, I thrive on hands-on projects and staying updated with industry trends. Skilled in coding, system administration, and cybersecurity, I love problem-solving and collaboration. Beyond technical expertise, I prioritize soft skills like communication and adaptability. Eager to contribute to the ever-evolving IT landscape, I'm excited about the possibilities technology holds for the future.</p>
                </div>
            </div>
         
        </div>  
    </section>
</div>
    </section>
  </MainLayout>
</template>