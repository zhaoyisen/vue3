<template>
  <div>
    <h2>{{ name }}</h2>
    <h2>{{ age }}</h2>
    <button @click="updateName">点击修改姓名</button>
    <button @click="updateAge">点击增加年龄</button>
    <button @click="showTel">点击查看电话</button>
  </div>
</template>

<script lang="ts">
export default {
    name:'Preson',
    data() {
        return{
        name:"张三",
        age:18,
        tel:"13887695123"
        }
    },
    methods: {
        updateName(){
            this.name="zhang-ssa";
        },
        updateAge(){
            this.age+=1;
        },
        showTel(){
            alert(this.tel)
        }
    }
}
</script>

<style lang="scss" scoped></style>