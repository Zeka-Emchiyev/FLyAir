<template>
  <div class="container">
    <h2 class="text-4xl my-6 text-[#5585e6] text-center ">FLYAIR TRAVEL TOURS</h2>
    <div class="grid lg:grid-cols-3 gap-4 m-2 ">
      <div v-for="tour in jsonData.tours" :key="tour.id" class="p-4 border rounded-lg hover:shadow-md transition">
        <img class="lg:w-full lg:h-[300px] rounded-lg mb-4" :src="require(`@/assets/${tour.img}`)" alt="FlyAir">
        <h4 class="text-2xl ">{{tour.name}}</h4>
        <p class="text-base text-[#535353] mb-4">{{tour.create}}</p>
        <span class="text-sm text-[#535353]">
          {{tour.content}}
        </span>
        <div class="flex mt-12">
          <div class="ml-auto">
            <p class="text-lg">From</p>
            <p class="text-sm text-[#535353]"> {{tour.price}}</p>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>
<script>
import jsonData from 'assets/data.json'
export default {
  name:'FormImage',
  data(){
    return {
      jsonData: jsonData,
    }
  }
}
</script>
