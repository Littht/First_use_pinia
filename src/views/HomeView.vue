<template>
    <h1>Home view: {{counterStore.counter}}</h1>
    <button @click="counterStore.incrementBy(1)">1</button>
    <button @click="counterStore.incrementBy(3)">3</button>
    <button @click="counterStore.incrementBy(5)">5</button>
    <button @click="counterStore.decrementBy(1)">-1</button>
    <h3>Numero de cambios: {{counterStore.numberOfChanges}}</h3>
</template>

<script setup>
    import { useCounterStore } from '../stores/counter';

    const counterStore= useCounterStore();

</script>