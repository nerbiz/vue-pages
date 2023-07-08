<script setup>
    import { reactive, ref } from 'vue';

    defineProps({
        mainTitle: String,
    });

    const counter = ref(0);

    function text() {
        return '<i>Text from function</i>';
    }
</script>

<template>
    <h2 class="text-xl font-bold">{{ mainTitle }}</h2>

    <h3 v-html="text()"></h3>

    <h4>Even 'slot' testen: <slot></slot></h4>

    <p>
        Current count: {{ counter }}
    </p>

    <p>
        <button class="border p-2 bg-gray-100 hover:bg-gray-200" @click="counter++">
            Increase count
        </button>
    </p>
</template>
