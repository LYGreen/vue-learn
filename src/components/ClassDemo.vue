<template>
    <h3>Class Style Binding</h3>
    <p :class="{ 'active': isActive, 'text-danger': hasError }">Class demo1</p>
    <p :class="classObject">Class demo2</p>
    <p :class="[ arrActive, arrHasError ]">Class demo3</p>
    <p :class="[ isActive ? 'active' : '']">Class demo4</p>
    <p :class="[ isActive ? 'active' : '', { 'text-danger': hasError }]">Class demo5</p>
</template>

<script>
export default {
    data() {
        return {
            isActive: true,
            hasError: true,
            classObject: {
                'active': true,
                'text-danger': true,
            },
            arrActive: "active",
            arrHasError: "text-danger",
        }
    }
}
</script>

<style>
.active {
    font-size: 30px;
}

.text-danger {
    color: red;
}
</style>
