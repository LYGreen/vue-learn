<template>
    <h3>Event Handle 5</h3>
    <button @click="addCount('Hello', $event)">Add</button>
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
        addCount(msg, e) {
            this.count++;
            e.target.innerHTML = "Add" + this.count;
            console.log(msg);
        }
    }
}

</script>
