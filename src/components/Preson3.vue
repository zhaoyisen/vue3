<template>
  <div>
    <h2>{{ name }}</h2>
    <h2>{{ age }}</h2>
    <button @click="updateName">点击修改姓名</button>
    <button @click="updateAge">点击增加年龄</button>
    <button @click="showTel">点击查看电话</button>
  </div>
</template>




<script setup lang="ts" name="Preson3" >
 import {ref} from 'vue';

let name =ref("张三323");
let age = ref(18);
let tel = "13887695123";
console.log("name",name)
console.log("age",age)

function updateName() {
  name.value = "zhang-ssa333";
}

function updateAge() {
  age.value += 1;
}

function showTel() {
  alert(tel);
}
</script>

<style lang="scss" scoped></style>