<template>
    <h3>Event Modifiers</h3>
    <a @click.prevent="clickHandle" href="localhost">Link</a>
    <div @click="clickDiv">
        <p @click.stop="clickP">Test</p>
    </div>
</template>

<script>
export default {
    data() {
        return {

        }
    },

    methods: {
        clickHandle(e) {
            //e.preventDefault();
            console.log("Clicked.");
        },
        clickDiv() {
            console.log("div");
        },
        clickP(e) {
            //e.stopPropagation();
            console.log("p");
        }
    }
}
</script>
