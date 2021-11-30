<template>
    <div class="banner">
        <h3>{{texto}}</h3>
    </div>
</template>

<script>
    export default {
        props:{
            texto:{
                type: String,
                default: "Pie de Pagina"
            }
        }
    }
</script>

<style scoped>
    .banner{
        color: red;
        
    }
</style>