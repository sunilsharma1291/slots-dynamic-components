<template>
    <div>
        <h3>Let's check it with the counter value</h3>
        <p>{{counter}}</p>
        <button @click = "counter++">Increase Counter</button>
    </div>
</template>

<script>
    export default {
        data(){
            return  {
                title: 'This is my red component',
                counter:0
            }
        },

        destroyed(){
            console.log('destroyed');
        },

        activated() {
            console.log('activated')
        },

        deactivated() {
            console.log('deactivated')
        },
    }
</script>

<style scoped>
    div {
        border:1px solid red;
    }
</style>