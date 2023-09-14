<template>
  <div
    class="relative h-screen w-full bg-no-repeat bg-cover bg-bottom bg-[url('https://images.pexels.com/photos/120049/pexels-photo-120049.jpeg')]">
    <div class="z-10 absolute w-full h-full flex justify-center items-center">
      <div class="text-center w-1/2">
        <h1 class="font-mono font-bold text-stone-200 text-5xl">Rent Your Adventure Today</h1>
        <!-- HOME SEARCH BAR Start-->
        <CarSearchBar />
        <!-- HOME SEARCH BAR End-->
      </div>
    </div>
    <div class="z-1 absolute w-full h-full bg-black opacity-50"></div>
  </div>
</template>