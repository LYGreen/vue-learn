<template>
    <h3>Event Handle 2</h3>
    <button @click="addCount">Add</button>
    <p>{{ count }}</p>
</template>

<script>
export default {
    data() {
        return {
            count: 0,
        }
    },

    methods: {
        addCount() {
            this.count++;
        }
    }
}
</script>
