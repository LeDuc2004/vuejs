<template>
    <h2>{{ message }}</h2>
    <h3>{{number + 5}}</h3>
</template>

<script>
    export default {
        data() {
            return {
                message: "hi there",
                number: 10
            }
        }
    }
</script>