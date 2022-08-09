<template>
    <h1>Counter view: {{counterStore.counter}}</h1>
    <button @click="counterStore.decrementBy(3)">-3</button>
    <h3>Numero de cambios: {{counterStore.numberOfChanges}}</h3>
</template>

<script setup>
    import { useCounterStore } from '../stores/counter';

    const counterStore = useCounterStore();
</script>