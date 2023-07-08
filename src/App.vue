<script setup>
    import Tester from './components/Tester.vue';
    import Toggle from './components/Toggle.vue';
</script>

<template>
    <h1 class="text-3xl font-bold">
        Hello world!
    </h1>

    <Tester main-title="Test title">
        Slot inhoud
    </Tester>

    <Toggle />
</template>
