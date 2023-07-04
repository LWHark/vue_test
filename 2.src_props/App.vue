<template>
    <div>
        <student name="张三" :age="18"/>
    </div>
</template>

<script>
import Student from './components/Student.vue'

export default {
    name: 'App',

    data() {
        return {
            
        };
    },

    components:{
        Student,
    }
};
</script>

<style lang="scss" scoped>

</style>