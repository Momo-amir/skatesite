<template>
    <div class="hero min-h-screen bg-black bg-cover" style="background-image: url(https://i.pinimg.com/originals/90/fa/ca/90faca2b99466f5b52dca565d5ba173d.jpg);">
     <div class="hero-overlay bg-opacity-60"></div>
     <div class="hero-content text-center text-white">
        <div class="max-w-md">
          <h1 class="mb-5 text-5xl font-bold">Find Your Spot</h1>
          <p class="mb-5">Search for street spots, skateparks, indoor skateparks, and transitions.</p>
        <form>
            <div class="relative z-10 flex space-x-3 p-1 bg-white rounded-lg">
                <div class="flex-[1_0_0%] ">
                    <label for="hs-search-article-1" class="block text-sm text-gray-700 font-medium bg-white outline-none"><span class="sr-only">Search article</span></label>
                    <input type="search" name="hs-search-article-1" id="hs-search-article-1" class="py-2.5 px-4 block w-full border-transparent rounded-lg" placeholder="Search for a spot">
                </div>
                <div class="flex-[0_0_auto]">
                    <button type="submit" class="size-[46px] inline-flex justify-center items-center gap-x-2 text-sm font-semibold border border-primary rounded-lg">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                            <path d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"/>
                        </svg>
                    </button>
                </div>
            </div>
        </form>
        <div class="mt-5 flex flex-wrap justify-center">
          <span class="inline-block bg-black text-white rounded px-3 py-1 text-sm font-semibold mr-2 mb-2 cursor-pointer" @click="searchTag('Street Spot')">Street Spot</span>
          <span class="inline-block bg-black text-white rounded px-3 py-1 text-sm font-semibold mr-2 mb-2 cursor-pointer" @click="searchTag('Skatepark')">Skatepark</span>
          <span class="inline-block bg-black text-white rounded px-3 py-1 text-sm font-semibold mr-2 mb-2 cursor-pointer" @click="searchTag('Indoor Skatepark')">Indoor Skatepark</span>
          <span class="inline-block bg-black text-white rounded px-3 py-1 text-sm font-semibold mr-2 mb-2 cursor-pointer" @click="searchTag('Transition')">Transition</span>
        </div>
     </div>
    </div>
    </div>
</template>

<script>
export default {
 methods: {
    searchTag(tag) {
      console.log(`Searching for: ${tag}`);
      // Implement your search logic here
    }
 }
}
</script>
