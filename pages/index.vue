<script lang="ts" setup>
definePageMeta({
    layout: "page"
})

const items = [
  '<img :src="/images/1.png">',
  '/1.png',
  '/1.png',
  '/1.png',
  '/1.png',
  '/1.png'
  
]

// const items = [
//   'https://picsum.photos/600/600?random=1',
//   'https://unsplash.com/photos/600/600?',
//   'https://picsum.photos/600/600?random=3',
//   'https://picsum.photos/600/600?random=4',
//   'https://picsum.photos/600/600?random=5',
//   'https://picsum.photos/600/600?random=6'
// ]

</script>
<template>
    <div>
        <section class="w-full flex-1 flex items-center justify-center gap-10 mt-24">
            <div class="w-1/2">
               <div class="">
                <h1><span class="text-[55px] text-black font-semibold">DISCOVER</span> <span class="text-[55px] text-gray-400 font-semibold">OUR</span><br>
                    <span class="text-[55px] text-black font-semibold">TRENDY</span> <span class="text-[55px] text-gray-400 font-semibold">AND</span><br>
                    <span class="text-[55px] text-black font-semibold">FRESH</span> <span class="text-[55px] text-gray-400 font-semibold">COLLECTION</span>
                </h1>
               </div>
               <div class="flex gap-4 w-1/2">
                <UButton :ui="{ rounded: 'rounded-full' }" color="black" variant="solid">get started</UButton>
                <UButton :ui="{ rounded: 'rounded-full' }" color="white" variant="solid">explore now</UButton>
               </div>
            </div>

            <div class="">
                <NuxtImg width="641px" height="656px" src="/images/fashionable-man-woman-sitting-stair 1.png" alt="preview"/>
            </div>
        </section>

        <section class="w-full flex-1 flex items-center justify-center gap-10 mt-24">
            <div class="w-1/2 flex-1 flex items-center justify-center">
                <NuxtImg width="370px" height="512px" src="/images/template.png" alt="preview"/>
            </div>

            <div class="w-1/2">
                <h1 class="text-5xl font-semibold">Welcome to Ophams</h1>
                <p class="text-4xl mt-3">Our mission is to empower<br>
                   individuals through fashion. We are<br>
                   committed to delivering exceptional<br>
                   quality and unparalleled service to<br>
                   our customers.</p>
            </div>
        </section>
 
        <section class="flex-1 flex items-center justify-between mt-24">
            <div class="">
                <h1 class="text-[64px] font-semibold">Our Collection</h1>
            </div>
            <div class="">
                <p class="text-2xl">Dare to be different, because<br> 
                   fashion shows you. What is<br>
                   happening. check out our collection!
                </p>
            </div>
        </section>

        <!-- test -->
        <!-- <section class="mt-24">
          <div>
            <h1>Image Slider Example</h1>
            <ImageSlider />
          </div>
        </section> -->

        <!-- Carousel -->
        <section class="mt-24">
            <UCarousel v-slot="{ item }" :items="items" :ui="{ item: 'basis-full md:basis-1/2 lg:basis-1/4' }" indicators class="rounded-lg overflow-hidden">
            <img :src="item" class="w-full" draggable="false">
            </UCarousel>
        </section>

        <section class="flex-col flex items-center justify-center mt-24">
            <div class="">
                <h1><span class="text-[64px] text-black font-semibold">Discover our</span> <span class="text-[64px] text-gray-400 font-semibold">durable</span> <span class="text-[64px] text-black font-semibold">and</span><br>
                    <span class="text-[64px] text-gray-400 font-semibold">resilient</span> <span class="text-[64px] text-black font-semibold">clothing materials</span></h1>
            </div>
            <div class="flex-1 flex justify-center items-center gap-4 mt-3">
                <div class="flex-col flex gap-4">
                    <NuxtImg src="/images/young-handsome-businessman-black-shirt-black-suit (1) 1.png" alt="preview"/>
                    <NuxtImg src="/images/male-female-walking-different-directions (1) 2.png" alt="preview"/>
                </div>
                <div>
                    <NuxtImg src="/images/portrait-young-japanese-woman-with-jacket 1.png" alt="preview"/>
                </div>
            </div>
            
        </section>

        <section class="flex-1 flex items-center justify-between my-24">
            <div class="">
                <h1 class="text-[64px] text-black font-semibold">Get In Touch</h1>
                <p class="text-2xl text-black font-semibold">Subscribe to our newsletter to<br>
                    get updates of our collections
                </p>
            </div>
            <div class="flex gap-2 justify-center items-center">
                <div>
                    <UInput :ui="{ rounded: 'rounded-full' }" color="gray" variant="outline" placeholder="Enter your email here" />
                </div>
                <div>
                    <UButton :ui="{ rounded: 'rounded-full' }" color="black" variant="solid">subscribe</UButton>
                </div>
            </div>
        </section>
    </div>
</template>