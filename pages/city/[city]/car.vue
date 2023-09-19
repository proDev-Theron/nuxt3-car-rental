<script setup>
const route = useRoute();
useHead({
    title: `Cars in ${route.params.city.toUpperCase()}`
})

definePageMeta({
    layout: "custom" //filename in layouts folder that will override the default layout
})

</script>

<template>
    <div>
        <div class="flex mt-32">
            <CarSidebar />
            <NuxtPage />
        </div>
    </div>
</template>