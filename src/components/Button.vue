<template>
    <button @click="AddTask()" :style="{background: color}" class="btn">{{text}}</button>
</template>

<script>
    export default {
        name: 'ButtonComp',
        props: {
            text: String,
            color: String
        },
        methods: {
            AddTask(){
                this.$emit('btn-click')
            },
        },
    }
</script>