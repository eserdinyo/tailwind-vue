<template>
  <div class="bg-dark w-full md:w-4/5 pt-6 px-10 md:py-16 md:px-24">
    <h4 class="text-font uppercase text-xs">Don't miss them</h4>
    <div class="mt-4">
      <div class="flex justify-between mb-4">
        <h4 class="text-white text-lg">Weekly quests</h4>
        <div class="flex items-center">
          <button class="btn mr-2">All Games</button>
          <div>
            <button class="px-3 py-2 mr-2 border-solid border-toggle border-2 rounded-lg">
              <img class="h-3" src="../assets/arrow-left.png" alt />
            </button>
            <button class="px-3 py-2 border-solid border-toggle border-2 rounded-lg">
              <img class="h-3" src="../assets/arrow-right.png" alt />
            </button>
          </div>
        </div>
      </div>
      <div class="overflow-x-auto md:flex">
        <Game v-for="quest in quests" :data="quest" :type="'quest'" />
      </div>
    </div>
    <h4 class="text-font uppercase text-xs mt-8">To The Top</h4>
    <div class="mt-2">
      <div class="flex justify-between items-center mb-8">
        <h4 class="text-white text-lg md:mb-8">Popular Games</h4>
        <div class="flex items-center">
          <button class="btn mr-2">All Games</button>
          <div>
            <button class="px-3 py-2 mr-2 border-solid border-toggle border-2 rounded-lg">
              <img class="h-3" src="../assets/arrow-left.png" alt />
            </button>
            <button class="px-3 py-2 border-solid border-toggle border-2 rounded-lg">
              <img class="h-3" src="../assets/arrow-right.png" alt />
            </button>
          </div>
        </div>
      </div>
      <div class="md:flex overflow-x-auto pt-4">
        <Game v-for="game in games" :data="game" :type="'game'" />
      </div>
    </div>
  </div>
</template>

<script>
import Game from "./Game";
import { games, quests } from "../data";
export default {
  data() {
    return {
      quests,
      games
    };
  },
  components: {
    Game
  }
};
</script>

<style lang="scss" scoped>
</style>