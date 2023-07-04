<template>
    <div>
        <h2>学生姓名：{{name}}</h2>
        <h2>学生年龄：{{age}}</h2>
        <h2>学生性别：{{sex}}</h2>
        <button @click="alertName">点我显示名称</button>
    </div>
</template>

<script>
import {mixin} from '../mixin'

export default {
    name: 'Student',

    // methods:{
    //     alertName(){
    //         alert(this.name)
    //     }
    // },

    mixins:[mixin],

    props:{
        name:{
            required:true,
        },
        age:{
            type:Number,
            default:18,
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