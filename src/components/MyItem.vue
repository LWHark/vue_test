<template>
    <li>
        <label>
            <input type="checkbox" :checked="todo.checked" @change="checkTodo(todo.id)"/>
            <span>{{todo.title}}</span>
        </label>
    </li>
</template>

<script>
export default {
    name: 'MyItem',

    props:['todo','checkTodo']
};
</script>

<style lang="css" scoped>
    li{
        list-style: none;
        height: 36px;
        line-height: 36px;
        padding: 0 5px;
        border-bottom: 1px solid #ddd;
    }
    li label{
        float: left;
        cursor: pointer;
    }
    li label li input{
        vertical-align: middle;
        margin-right: 6px;
        position: relative;
        top: -1px;
    }
    li button{
        float: right;
        display: none;
        margin-top: 3px;
    }
    li:before{
        content: initial;
    }
    li:last-child{
        border-bottom: none;
    }
    li:hover button{
        display: block;
    }
</style>