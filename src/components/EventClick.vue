<template>
   <button @click="ShowMessage(100)">onclick</button>
</template>

<script>
    export default {
        data() {
            return {
                message: "hi there",
                number: 10
            }
        },
        methods: {
            ShowMessage(input) {
                alert(input)
            }
        }
    }
</script>