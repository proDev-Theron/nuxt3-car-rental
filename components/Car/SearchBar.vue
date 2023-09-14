<script setup>
const city = ref("");
const cityError = ref(false);

const handleSearch = () => {
  if(!city.value){
    return cityError.value = true;
  }
  navigateTo(`/city/${city.value}/car`);
};
</script>

<template>
  <div class="flex border rounded-full justify-between overflow-hidden mt-4 mx-auto">
    <input type="text"
      class="focus:outline-none py-2 px-4 w-full text-gray-200 placeholder-gray-200 bg-transparent"
      :class="cityError ? 'border border-red-500': ''"
      placeholder="Search for your dream car..."
      v-model="city">
    <button class="bg-gray-500 text-white px-10" @click="handleSearch">Search </button>
  </div>
</template>