<script setup>
const route = useRoute();
const { toTitleCase } = useUtilities();
const { cars } = useCars();

useHead({
    title: toTitleCase(route.params.name),
});

definePageMeta({
    layout: "custom"
});

const car = computed(() => {
    return cars.find((c) => {
        return c.id === parseInt(route.params.id);
    })
});

if (!car.value) {
    throw createError({
        statusCode: 404,
        message: `Car with ID ${route.params.id} does not exist`
    })
}

</script>

<template>
    <div v-if="car">
        <CarDetailHero :car="car" />
        <CarDetailAttributes :features="car.features" />
        <CarDetailDescription :description="car.description" />
        <CarDetailContact />
    </div>
</template>