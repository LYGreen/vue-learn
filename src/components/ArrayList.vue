<template>
    <h3>Array change monitoring</h3>
    <button @click="addListHandle">Add data</button>
    <ul>
        <li v-for="(item, index) in names" :key="index">{{ item }}</li>
    </ul>
    <button @click="concatArrayHandle">Concat array</button>
    <h3>Array 1</h3>
    <span v-for="item in arr1">{{ item }}&nbsp;</span>
    <h3>Array 2</h3>
    <span v-for="item in arr2">{{ item }}&nbsp;</span>
    <h3>Final array</h3>
    <span>{{ finalArray }}</span>
</template>

<script>
export default {
    data() {
        return {
            names: ["anna", "flower", "snow"],
            arr1: [1, 2, 3, 4, 5],
            arr2: [6, 7, 8, 9, 10],
            finalArray: []
        }
    },

    methods: {
        addListHandle() {
            //this.names.push("sakura");
            this.names = this.names.concat(["sakura"]);

            console.log(this.names);
        },
        concatArrayHandle() {
            this.finalArray = this.arr1.concat(this.arr2);
        }
    }
}
</script>
