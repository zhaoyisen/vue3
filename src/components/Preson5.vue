<template>
  <div>
    <h1>一辆{{ car.brand }}车，价值{{ car.price }}万</h1>
    <button @click="updateCarPrice">更新价格</button>

    <hr />
    <li v-for="game in games" :key="game.id">
      {{ game.name }}
    </li>
    <button @click="uploadGame">游戏更新</button>

    <hr />
    <h2>测试：{{ a.b.c.d.e.f }}</h2>
    <button @click="test">test</button>
  </div>
</template>




<script setup  lang="ts" name="Preson5">
  import { ref } from 'vue';
let car = ref({
  brand: "奔驰",
  price: 100
})

let games = ref([
  {
    id: "001",
    name: "csgo"
  },
  {
    id: "002",
    name: "valuer"
  },
  {
    id: "003",
    name: "dnf"
  }
])


let a = ref({
  b: {
    c: {
      d: {
        e: {
          f: 500
        }
      }
    }
  }
})
console.log(a)

function test(){
  a.value.b.c.d.e.f=999;


}


function updateCarPrice() {
  car.value.price += 1;
}



function uploadGame() {
  games.value[0].name = "cs2";



}

</script>

<style lang="scss" scoped></style>