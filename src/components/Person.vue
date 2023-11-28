<script lang="ts">
    import { defineComponent } from 'vue';
    import type { PropType } from 'vue';
    
    interface Person {
        name: string,
        email: string,
        age: number
    }
    
    export default defineComponent({
        props: {
            person: {
                type: Object as PropType<Person>,
                required: true
            }
        }
    })
</script>

<template>
    <div>
        <h2>Person info</h2>
        <p><b>Name:</b> {{ person.name}}</p>
        <p><b>Email:</b> {{ person.email}}</p>
        <p><b>Age:</b> {{person.age}}</p>
    </div>
</template>