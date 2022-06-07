<template>
    <h3>{{this.text}} </h3>
</template>

<script>
export default {
    name: 'My-Task',

    props: {
        task: Object,
    },
}
</script>