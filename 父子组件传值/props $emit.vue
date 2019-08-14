<!--父组件-->
<!--静态props-->
<button msg="hello"></button>

<!--动态props-->
<!--父组件： 要动态地绑定父组件的数据到子模板的props用
v-bind 每当父组件的数据变化的时候 该变化也会传给子组件-->
<!--3.单项数据流-->
<!--prop 是单向绑定的：当父组件的属性变化时，将传导给子组件，但是不会反过来。这是为了防止子组件无意修改了父组件的状态-->
<!--另外，每次父组件更新时，子组件的所有 prop 都会更新为最新值。这意味着你++不应该在子组件内部改变 prop++ .-->

<!--动态绑定-->
<button :msg="hello"></button>

<template>
    <div>{{msg}}</div>
    <!--输出hello-->
</template>


<script>
    export default {
        name: "props $emit",
        props:['msg']
    }
</script>

<style scoped>

</style>