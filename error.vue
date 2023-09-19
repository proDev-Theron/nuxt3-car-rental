<script setup>
const error = useError();
const handleError = () => {
    clearError({
        redirect: "/"
    });
}

</script>
<template>
    <div class="flex h-screen justify-center items-center flex-col">
        <h1 class="text-9xl text-blue-500 font-bold">{{error.statusCode}}</h1>
        <p class="text-xl">{{error.message}}</p>
        <button @click="handleError" class="rounded mt-7 text-2xl bg-blue-500 px-7 py-4 text-white">Go to Home</button>
    </div>
</template>