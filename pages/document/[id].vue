<template>
    <div>
        <p>Documnent details for id = {{ id }}</p>
        <p>More text</p>
    </div>
</template>

<script setup>
const { id } = useRoute().params
</script>

<style scoped>

</style>