<template>
<section>
    <div :key="task.id" v-for="task in tasks">
        <h3>
            {{task.text}}
        </h3>   
    </div>  
</section>  
</template>

<script>
export default{
    name: 'My-Tasks',

    props: {
        tasks: Array,
    }
}
</script>
