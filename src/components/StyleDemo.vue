<template>
    <h3>Style Demo</h3>
    <p :style="{ color: 'red' }">Style binding</p>
    <p :style="{ color: 'red', fontSize: 30 + 'px' }">Style binding</p>
    <p :style="{ color: activeColor }">Style binding</p>
    <p :style="styleObject">Style binding</p>
    <p :style="[styleObject]">Style binding</p>
</template>

<script>

export default {
    data() {
        return {
            activeColor: 'green',
            styleObject: {
                color: 'red',
                // fontSize: 35 + 'px',
                fontSize: '35px',
            }
        }
    }
}

</script>
