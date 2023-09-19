<script setup>
const {cars} = useCars();
</script>

<template>
    <div class="w-[1/2]">
        <CarCard v-for="car in cars" :key="car.id" :car="car"/>
    </div>
</template>