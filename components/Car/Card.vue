<script setup>
const props = defineProps({
    car: {
        type: Object,
        
    }
})
</script>

<template>
    <div class="shadow border w-full overflow-hidden mb-5 cursor-pointer h-[1/2]" @click='navigateTo(`/car/${car.name}-${car.id}`)'>
        <div class="flex h-full">
            <img :src="car.url" 
                  class="w-[300px] h-full">
            <div class="p-4 flex flex-col">
                <div>
                    <h1 class="text-2xl text-blue-400">{{ car.name }}</h1>
                    <p class="text-gray-700">{{ car.description }}</p>
                </div>
                <div class="mt-auto text-xl">${{ car.price }}</div>
            </div>
        </div>
    </div>
</template>