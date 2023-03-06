<template>
  <div class="container  contain m-5">
    <h1 class="text-center">Converter</h1>
    <div class="main">
      <h4><i> Select Category</i></h4>
      <select v-model="category" class="form-control select">
        <option value="default" placeholder="select" selected>Select Category</option>
        <option value="mass">Mass</option>
        <option value="area">Area</option>
        <option value="len">Length</option>
        <option value="temp">Temperature</option>
        <option value="data">Data Transfer Rate</option>
        <option value="vol">Volume</option>
        <option value="speed">Speed</option>
      </select>
    </div>
    <Area v-show="comp_show.area" />
    <Data v-show="comp_show.data" />
    <Speed v-show="comp_show.speed" />
    <Temperature v-show="comp_show.temp" />
    <Volume v-show="comp_show.vol" />
    <Length v-show="comp_show.len" />
    <Mass v-show="comp_show.mass" />
  </div>
</template>
<script>
import Area from './components/Area.vue';
import Data from './components/Data.vue';
import Speed from './components/Speed.vue';
import Volume from './components/Volume.vue';
import Length from './components/Length.vue';
import Temperature from './components/Temperature.vue';
import Mass from './components/Mass.vue';

import './assets/bootstrap/bootstrap.bundle.min.js'
import './assets/bootstrap/bootstrap.min.js'
export default {
  data() {
    return {
      category: "default",
      comp_show: {
        mass: false,
        len: false,
        speed: false,
        temp: false,
        area: false,
        data: false,
        vol: false,
      }
    }
  },
  components: {
    Area,
    Data,
    Speed,
    Volume,
    Length,
    Temperature,
    Mass

  },
  watch: {
    category(value) {
      this.comp_show.mass = false,
        this.comp_show.len = false,
        this.comp_show.speed = false,
        this.comp_show.temp = false,
        this.comp_show.data = false,
        this.comp_show.vol = false,
        this.comp_show.area = false
      this.comp_show[value] = true; {
        console.log(">>>", this.comp_show)
      }
      console.log(">>>", value)
    }
  }
}

</script>
<style>
@import url('@/assets/bootstrap/bootstrap.min.css');
</style>