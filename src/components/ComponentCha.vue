<template>
    <ComponentCon :message="message"/>
 </template>
 
 <script>
    import ComponentCon from "./ComponentCon.vue";
     export default {
        components: {
            ComponentCon
        },
         data() {
             return {
                 message: "Tình cha ấm áp như vần thái dương",
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