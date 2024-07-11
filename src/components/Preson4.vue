<template>
  <div>
    <h1>一辆{{ car.brand }}车，价值{{ car.price }}万</h1>
    <button @click="updateCarPrice">更新价格</button>

<hr/>
    <li v-for="game in games" :key="game.id">
      {{ game.name }}
    </li>
    <button @click="uploadGame">游戏更新</button>

  </div>
</template>




<script setup lang="ts" name="Preson4" >
 import {reactive, ref} from 'vue';
  let car=reactive({
    brand:"奔驰",
    price:100
  })


let games=reactive([
  {
    id:"001",
    name:"csgo"
  },
  {
    id:"002",
    name:"valuer"
  },
  {
    id:"003",
    name:"dnf"
  }
])


  console.log("car",car)

  function updateCarPrice(){
    car.price+=1;
  }
  


  function uploadGame(){
    games[0].name="cs2";



  }

</script>

<style lang="scss" scoped></style>