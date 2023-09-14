<script setup>
const route = useRoute();
useHead({
    title: `Cars in ${route.params.city.toUpperCase()}` 
})
</script>

<template>
    <div>
        <NavBar />
        <div class="mx-auto mt-4 max-w-7xl space-y-4 px-4 pb-16 w-[full] xs:px-8 sm:px-10 lg:px-16">
            <div class="flex mt-32">   
                <CarSidebar />
                <NuxtPage />
            </div>
        </div>
    </div>
</template>