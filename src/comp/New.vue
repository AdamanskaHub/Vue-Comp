<template>
    <div>
        <h3>New quote</h3>
        <button @click="counter++">Count</button>
        <p>{{ counter }}</p>
    </div>
  
</template>

<script>
    export default {
        data: function() {
            return {
                counter: 0,
            };
        }
    }
</script>

<style scoped>
</style>
