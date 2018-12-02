<template>
    <div>
        {{ title }}
    </div>
</template>

<script>
    export default {
        data(){
            return  {
                title: 'This is my blue component'
            }
        }
    }
</script>

<style scoped>
    div {
        border:1px solid blue;
    }
</style>