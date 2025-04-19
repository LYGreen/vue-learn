<template>
    <h3>Property Binding</h3>
    <div v-bind:id="dynamicId" v-bind:class="dynamicClass">test</div>
    <button :disabled="isButtonDisabled">button</button>
    <div v-bind="objectOfAttrs">test</div>
</template>

<script>
export default {
    data() {
        return {
            dynamicId: "myId",
            dynamicClass: "myClass",
            dynamicTitle: undefined,
            isButtonDisabled: false,
            objectOfAttrs: {
                class: "myClass",
                id: "myId"
            }
        }
    }
}
</script>

<style>
.myClass {
    color: red;
    font-size: 30px;
}
</style>
