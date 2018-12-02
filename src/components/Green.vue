<template>
    <div>
        {{ title }}
    </div>
</template>

<script>
    export default {
        data(){
            return  {
                title: 'This is my green component'
            }
        }
    }
</script>

<style scoped>
    div {
        border:1px solid green;
    }
</style>