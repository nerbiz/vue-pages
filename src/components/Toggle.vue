<template>
    <div>
        <button @click="isHidden = !isHidden">Toggle Elements</button>

        <div :class="{ hidden: isHidden }">Element 1</div>
        <div :class="{ hidden: isHidden }">Element 2</div>
        <div :class="{ hidden: isHidden }">Element 3</div>
        <div :class="{ hidden: isHidden }">Element 4</div>
    </div>
</template>

<script setup>
    import { ref } from 'vue';

    const isHidden = ref(true);
</script>
