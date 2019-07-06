<template>
  <div class="md:mr-4 mb-8 gameMinWidth mx-auto">
    <div class="relative" v-if="type=='quest'">
      <div class="h-xl w-full rounded-t-lg overflow-hidden">
        <img class="h-full w-full" :src="data.image" alt />
      </div>
      <button
        class="btn absolute top-0 left-0 mt-6 ml-6 text-xs px-3 py-1 rounded-sm overflow-hidden"
      >Action</button>
    </div>
    <div class="p-4 bg-game h-24" v-if="type=='quest'">
      <h4 class="text-white font-semibold">{{ data.name }}</h4>
      <p class="text-font text-sm mt-2">{{data.desc}}</p>
    </div>

    <div class="bg-game relative h-24  rounded-t-lg" v-if="type=='game'">
      <div class="absolute -mt-4 ml-4 h-20 w-20 rounded-lg overflow-hidden">
        <img class="h-full w-full" :src='data.image' alt />
      </div>
      <div class="absolute right-0 mt-4 mr-16 md:mr-4">
        <h4 class="text-white font-semibold">{{data.name}}</h4>
        <p class="text-font text-sm mt-2">{{data.desc}}</p>
      </div>
      <button
        class="btn absolute bottom-0 left-0 ml-6 mb-6 text-xs px-3 py-1 rounded-lg overflow-hidden"
      >Action</button>
    </div>
    <!-- bottom -->
    <div
      class="flex items-center px-2 py-3 bg-game border-solid border-gameBorder border-t rounded-b-lg"
    >
      <div class="flex items-center -m-2">
        <img src="../assets/coin.png" class="w-12" alt />
        <p class="text-white text-sm -m-1">{{data.coin}}</p>
      </div>
      <div class="flex items-center ml-2">
        <img src="../assets/energy.png" class="w-12" alt />
        <p class="text-white text-sm -ml-1">{{data.energy}}</p>
      </div>
      <button class="btn ml-auto py-1 text-xs">Accept</button>
    </div>
  </div>
</template>

<script>
export default {
  props: ["type", "data"]
};
</script>