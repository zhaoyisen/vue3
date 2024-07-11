<template>

    <!-- html结构 -->
    <div class="app">
        <!-- <h1>test</h1> -->
        <!-- <PresonVue></PresonVue> -->
        <!-- <PresonVue3></PresonVue3> -->
        <!-- <PresonVue4></PresonVue4> -->
        <!-- <PresonVue5></PresonVue5> -->
        <Antd1></Antd1>

    </div>



</template>


<script lang="ts">
import PresonVue from './components/Preson.vue'
import PresonVue3 from './components/Preson3.vue'
import PresonVue4 from './components/Preson4.vue'
import PresonVue5 from './components/Preson5.vue'
import Antd1 from './components/Antd1.vue'




export default {

    name: "App",
    components: { PresonVue, PresonVue3, PresonVue4, PresonVue5, Antd1 }
}


// js或者ts

</script>


<style>
/* 样式 */
</style>