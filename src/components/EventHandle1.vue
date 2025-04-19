<template>
    <h3>Event Handle 1</h3>
    <button v-on:click="count++">Add</button>
    <p>{{ count }}</p>
</template>

<script>
export default {
    data() {
        return {
            count: 0,
            count2: 0,
        }
    },
}
</script>
