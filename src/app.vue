<!-- 布局文件 -->
<template>
    <img src="./assets/logo.png" />
    <h1>{{msg}}</h1>
    <comp-a></comp-a>
    <comp-b></comp-b>
    <counter></counter>
</template>
<style>
    body{
        background-color:#f7f7f7;
    }
</style>

<script>
    import CompA from './components/a.vue'
    import CompB from './components/b.vue'
    import Counter from './components/counter.vue'
    export default {
        data () {
            return {
                msg: 'data from vue-loader'
            }
        },
        components: {
            CompA,
            CompB,
            Counter
        }
    }
</script>

