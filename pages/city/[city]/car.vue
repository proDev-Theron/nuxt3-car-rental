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
            <NuxtErrorBoundary>
                <CarSidebar />
                <NuxtPage />
                <template #error="{error}">
                    <div class="text-center flex flex-col mx-auto">
                        <h1 class="text-5xl text-red-600 mb-4">Something went wrong</h1>
                        <code>{{ error }}</code>
                        <button class="text-white bg-blue-400 px-10 py-4 rounded mt-4" @click="error.value=null">Try Again</button>
                    </div>
                </template>
            </NuxtErrorBoundary>
        </div>
    </div>
</template>