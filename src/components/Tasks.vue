<template>
<section>
    <div :key="task.id" v-for="task in tasks">
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
    }
}
</script>
