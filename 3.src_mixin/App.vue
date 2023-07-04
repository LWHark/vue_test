<template>
    <div>
        <school name='中南大学' address='长沙左家垅'></school>
        <hr>
        <student name='张三'></student>
    </div>
</template>

<script>
import Student from './components/Student.vue'
import School from './components/School.vue'

export default {
    name: 'App',
    components:{
        Student,
        School,
    }
};
</script>

<style lang="scss" scoped>

</style>