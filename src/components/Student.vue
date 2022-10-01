<template lang="">
    <div>
        <h1>{{msg}}</h1>
        <h2>姓名：{{name}}</h2>
        <h2>性别：{{gender}}</h2>
        <h2>年龄：{{age+1}}</h2>
    </div>
</template>
<script>
export default {
    name: 'Studeng',
    data() {
        return {
            msg:"我是一名同济大学的学生！"
        }
    },
    props: {
        name: {
            tyep: String,
            required:true
        },
        age: {
            tyep: Number,
            required: true,
            default:18
        },
        gender: {
            tyep: String,
            required:false
        },
    }
}
</script>
<style lang="">
    
</style>