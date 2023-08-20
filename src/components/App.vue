<template>
    <div class="container h-100 d-flex justify-content-center align-items-center">
        <div class="card rounded-5 text-bg-dark">
            <div class="card-body p-5">
                <div class="d-flex flex-column align-items-center">
                    <div class="mb-4">
                        <img src="/favicon.svg" class="img-fluid">
                    </div>
                    <h1 class="fw-bold">{{ title }}</h1>
                    <p class="fw-bold">Open your favorite code editor and start working on your project!</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
#app {
    background-color: #FFFFFF;
}
</style>

<script setup>
import { ref, onMounted } from 'vue';

const title = ref(null);

onMounted(() => {
    title.value = 'Everything is fine!';
});
</script>