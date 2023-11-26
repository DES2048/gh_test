<script lang="ts">
    import { defineComponent } from 'vue';

    export default defineComponent({
        props: {
            name: {
                type:String,
                required:true
            }
        },
        mounted() {
            const k = this.name;
        }
    })
</script>

<template>
    <h2>Hello, {{name}}!</h2>
</template>