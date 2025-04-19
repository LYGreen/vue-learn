<template>
    <h3>List Rendering</h3>
    <p v-for="item in items">{{ item }}</p>
    <p v-for="item of items">{{ item }}</p>
    <p v-for="(item, index) in items">{{ index }}: {{ item }}</p>
    <p v-for="(item, key, index) in obj">{{ index }}. {{ key }}: {{ item }}</p>
</template>

<script>
export default {
    data() {
        return {
            items: ["apple", "pear", "watermalon"],
            obj: {
                id: 1,
                name: "myname",
                bio: "null"
            }
        }
    }
}
</script>
