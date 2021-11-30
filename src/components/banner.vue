<template>
    <div class="banner">
        <h2>{{texto}}</h2>
    </div>
</template>

<script>
    export default {
        props:{
            texto:{
                type: String,
                default: "Texto Default"
            },
            imagen:{
                type: String,
                default: ""
            }
        }
    }
</script>

<style scoped>
    .banner{
        background: greenyellow;
        color: red;
    }
</style>