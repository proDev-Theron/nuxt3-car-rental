<template>
  <div>
    <!-- NAVBAR Start -->
    <header class="sticky top-0 z-50 flex justify-between items-center space-x-1 border-b bg-white p-4 shadow-md">
      <a class="text-3xl font-mono" href="">car rental</a>
    </header>
    <!-- NAVBAR End -->

    <!-- CARS PAGE Start -->
    <div class="mx-auto mt-4 max-w-7xl space-y-4 px-4 pb-16 w-3/5 xs:px-8 sm:px-10 lg:px-16">
      <div class="flex mt-32">
        <!-- CAR Sidebar Start -->
        <div class="shadow border w-64 mr-10 z-30 h-[190px]">
          <div class="relative flex justify-between p-5 cursor-pointer border-b">
            <h3>Location</h3>
            <h3 class="text-blue-400 capitalize">Toronto</h3>
            <!-- <div class="absolute border shadow left-56 p-5 top-1 m-1 bg-white">
              <input type="text" class="border p-1 rounded">
              <button class="bg-blue-400 w-full mt-2 rounded text-white p-1">Apply</button>
            </div> -->
          </div>
          <div class="relative flex justify-between p-5 cursor-pointer border-b">
            <h3>Make</h3>
            <h3 class="text-blue-400 capitalize">Toyota</h3>
          </div>
          <div class="relative flex justify-between p-5 cursor-pointer border-b">
            <h3>Price</h3>
            <h3 class="text-blue-400 capitalize">Any</h3>
          </div>
        </div>
        <!-- CAR Sidebar End -->

        <!-- CAR Cards Start -->

        <!-- CAR Cards End -->
      </div>
    </div>
    <!-- CARS PAGE End -->
  </div>
</template>
