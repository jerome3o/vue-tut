<script lang="ts">
export default {
    // Properties returned from data() become reactive state
    // and will be exposed on `this`.
    data() {
        return {
            count: 0
        }
    },

    // Methods are functions that mutate state and trigger updates.
    // They can be bound as event listeners in templates.
    methods: {
        increment() {
            this.count++
        }
    },

    // Lifecycle hooks are called at specific points in the component lifecycle.
    // They can be used to perform side effects, such as fetching data.
    mounted() {
        console.log(`The initial count is ${this.count}.`)
    }
}
</script>

<template>
    <button @click="increment">
        Count is: {{ count }}
    </button>
</template>
