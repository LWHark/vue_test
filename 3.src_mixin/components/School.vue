<template>
    <div>
        <h2>学校姓名：{{name}}</h2>
        <h2>学校地址：{{address}}</h2>
        <button @click="alertName">点我显示名称</button>
    </div>
</template>

<script>
import {mixin} from '../mixin'

export default {
    name: 'School',

    data() {
        return {
            
        };
    },

    // methods: {
    //     alertName(){
    //         alert(this.name)
    //     }
    // },

    mixins:[mixin],

    props:{
        name:{
            required:true,
            type:String,
        },
        address:{
            required:true,
            type:String
        }
    }
};
</script>

<style lang="scss" scoped>

</style>