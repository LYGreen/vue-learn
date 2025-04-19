<template>
    <h3>模板语法</h3>
    <p>{{ msg }}</p>
    <p>{{ number + 1 }}</p>
    <p>{{ ok ? 'Yes' : 'No' }}</p>
    <p>{{ message.split("").reverse().join("") }}</p>
    <p>{{ rawHtml }}</p>
    <p v-html="rawHtml"></p>
</template>

<script>
export default {
    data() {
        return {
            msg: "Hello World !",
            number: 0,
            ok: true,
            message: "Hello",
            rawHtml: "<a href='http://localhost:5173'>Link</a>",
        }
    }
}
</script>
