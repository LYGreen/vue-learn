<template>
    <h3>Conditional Rendering</h3>
    <div v-if="flag">flag is true</div>
    <div v-else>flag is false</div>

    <div v-if="type === 'A'">A type</div>
    <div v-else-if="type === 'B'">A type</div>
    <div v-else-if="type === 'C'">A type</div>
    <div v-else>Not A/B/C</div>

    <div v-show="flag">test v-show</div>
</template>

<script>
export default {
    data() {
        return {
            flag: true,
            type: 'D',
        }
    }
}
</script>
