<template>
    <h1>I am a Counter Component. Edit me in dev mode.</h1>
    <p>Current Count: {{count}}</p>
</template>

<script>
    export default {
        data () {
            return {
                count: 0
            }
        },
        ready () {
            this.handle = setInterval(() => {
                this.count++;
            }, 1000)
        },
        destroyed () {
            clearInterval(this.handle);
        }
    }
</script>