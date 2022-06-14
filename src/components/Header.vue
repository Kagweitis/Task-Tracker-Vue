<template>
    <header>
        <h1>
            Task Tracker
        </h1>
        <Button @toggle-add-task="$emit('toggle-add-task')" 
        text="Add Task" color="green" />
    </header>    
</template>

<script>

import Button from './Button'

export default{
    name: 'My-Header',

    components: {
        Button
    },
}
</script>

<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>
