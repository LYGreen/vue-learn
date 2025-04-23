<template>
    <h3>computed demo</h3>
    <!-- Compute once -->
    <p>{{ objComputed }}</p>
    <p>{{ objComputed }}</p>
    <p>{{ objComputed }}</p>
    <p>{{ objComputed }}</p>
    <!-- Compute 4 times -->
    <p>{{ objMethod() }}</p>
    <p>{{ objMethod() }}</p>
    <p>{{ objMethod() }}</p>
    <p>{{ objMethod() }}</p>
</template>

<script>
export default {
    data() {
        return {
            obj: {
                name: "sakura",
                content: ["pink", "flower", "leaf"]
            }
        }
    },

    computed: {
        objComputed() {
            return this.obj.name.length > 0 ? "Yes" : "No"
        }
    },

    methods: {
        objMethod() {
            return this.obj.name.length > 0 ? "Yes" : "No"
        }
    }
}
</script>
