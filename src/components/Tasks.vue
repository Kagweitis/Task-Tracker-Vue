<template>
<section>
    <div @toggle-reminder="$emit('toggle-reminder', task.id)" @delete-task="$emit('delete-task', task.id)" 
    :key="task.id" v-for="task in tasks">
        <Task :task="task" />
    </div>  
</section>  
</template>

<script>
import Task from './Task'

export default{
    name: 'My-Tasks',

    props: {
        tasks: Array,
    },

    components:{
        Task,
    },
    emits:['toggle-reminder', 'delete-task']
}
</script>

