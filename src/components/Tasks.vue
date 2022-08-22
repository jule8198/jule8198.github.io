<template>
    <div :key="task.id" v-for="task in tasks">
        <Taskvue :task ="task" />
    </div>
</template>

<script>
import TaskVue from './Task.vue';

export default {
    name: 'Tasks',
    props: {
        tasks: Array,
    },
    components: {
        TaskVue,
    }
}
</script>

<style lang="scss" scoped>

</style>