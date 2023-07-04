<template>
    <div>
        <h2>学生名称：{{name}}</h2>
        <h2>学生年龄：{{myAge+1}}</h2>
        <h2>学生性别：{{sex}}</h2>
        <h2>学生信条：{{remark}}</h2>
        <button @click="changeAge">点我增加年龄</button>
    </div>
</template>

<script>
export default {
    name: 'Student',

    data() {
        return {
            remark:'君子以自强不息！',
            myAge:this.age,
        };
    },
    methods:{
        changeAge(){
            this.myAge++;
        }
    },
    // props:['name','age','sex']
    props:{
        name:{
            required:true,
        },
        age:{
            type:Number,
            required:true
        },
        sex:{
            type:String,
            default:'保密'
        }
    }
};
</script>

<style lang="scss" scoped>

</style>