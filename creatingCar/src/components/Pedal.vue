<template>
    <button @click="accion()">{{msg}}</button>
</template>
<script>
    export default {
        props: {
            msg : String
        },
        methods: {
            accion (){
                this.$emit('action')
            }
        }
    }
</script>
