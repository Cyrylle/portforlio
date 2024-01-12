<script setup>
import JavascriptLogo from '../assets/javascript-logo-big.png';

</script>

<template>
    <div class="bg-white py-6 sm:py-8 lg:py-12">
        <div class="mb-4 flex flex-col items-center md:mb-8 lg:flex-row lg:justify-between">
            <h2 class="mb-2 text-center font-serif text-2xl font-bold text-purple-800 lg:mb-0 lg:text-3xl">Technology Stacks</h2>
            
        </div>

        <!-- Technology Stacks -->
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 rounded-lg md:grid-cols-3 lg:gap-6">
            <!-- logo - start -->
            <div class="flex h-16 items-center justify-center rounded-lg bg-gray-100 p-4 text-gray-400 sm:h-32">
                <img class="w-18 lg:w-24 h-full object-fit" :src="JavascriptLogo" alt="Javascript">
            </div>
            <!-- logo - end -->

             <!-- logo - start -->
             <div class="flex h-16 items-center justify-center rounded-lg bg-gray-100 p-4 text-gray-400 sm:h-32">
                <img class="w-18 lg:w-24 h-full object-fit" src="../assets/html.jpg" alt="HTML">
            </div>
            <!-- logo - end -->
             <!-- logo - start -->
            <div class="flex h-16 items-center justify-center rounded-lg bg-gray-100 p-4 text-gray-400 sm:h-32">
                <img class="w-18 lg:w-24 h-full object-fit" src="../assets/css.jpg" alt="HTML">
            </div>
            <!-- logo - end -->
            <!-- logo - start -->
            <div class="flex h-16 items-center justify-center rounded-lg bg-gray-100 p-4 text-gray-400 sm:h-32">
                <img class="w-18 lg:w-24 h-full object-fit" src="../assets/vue.png" alt="HTML">
            </div>
            <!-- logo - end -->
             <!-- logo - start -->
             <div class="flex h-16 items-center justify-center rounded-lg bg-gray-100 p-4 text-gray-400 sm:h-32">
                <img class="w-18 lg:w-24 h-full object-fit" src="../assets/lara.png" alt="HTML">
            </div>
            <!-- logo - end -->
             <!-- logo - start -->
             <div class="flex h-16 items-center justify-center rounded-lg bg-gray-100 p-4 text-gray-400 sm:h-32">
                <img class="w-18 lg:w-24 h-full object-fit" src="../assets/php.png" alt="HTML">
            </div>
            <!-- logo - end -->

            
        </div>
    </div>
</template>