<template>
    <h3>Event Handle 4</h3>
    <button @click="addCount('Hello')">Add</button>
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
        addCount(msg) {
            this.count++;
            console.log(msg);
        }
    }
}

</script>
