<template>
    <div>
        <h2>学校名称：{{name}}</h2>
        <h2>学校地址：{{address}}</h2>
    </div>
</template>

<script>
export default {
    name: 'School',

    data() {
        return {
          name:'中南大学',
          address:'长沙左家垅'  
        };
    }
};
</script>

<style lang="scss" scoped>

</style>