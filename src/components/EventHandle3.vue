<template>
    <h3>Event Handle 3</h3>
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
        addCount(e) {
            this.count++;
            e.target.innerHTML = "Add" + this.count;
        }
    }
}

</script>
