<script setup>
const route = useRoute();

const { toTitleCase } = useUtilities();

useHead({
    title: `${route.params.make ? toTitleCase(route.params.make) : "Cars"} in ${toTitleCase(route.params.city)}`,
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