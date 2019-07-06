<template>
  <div class="bg-dark2 w-1/5 py-8  flex flex-col">
    <div class="flex items-center justify-between text-white mb-6 px-8 cursor-pointer">
      <p>GAMES</p>
      <div>
        <img class="h-2" src="../assets/arrow.png" alt />
      </div>
    </div>
    <div class="text-white mb-6 font-light px-8 cursor-pointer">
      <p>All Games</p>
    </div>
    <div>
      <div @click="isNavOpen = !isNavOpen" class="flex justify-between items-center mb-6 px-8 cursor-pointer">
        <p class="text-white">Categories</p>

        <img class="h-2" src="../assets/arrow.png" alt />
      </div>
      <ul :class="{toggleNav:isNavOpen}" class="text-font select-none">
        <li
          class="flex cursor-pointer items-center py-4 px-10 bg-dark3 border-solid border-indigo-700 border-l-4"
        >
          <div class="ml-4 mr-6">
            <img class="h-5" src="../assets/action.png" alt />
          </div>
          <p>Action</p>
        </li>
        <li class="flex cursor-pointer py-4 px-10">
          <div class="ml-4 mr-6">
            <img class="h-5" src="../assets/adventure.png" alt />
          </div>
          <p>Adventure</p>
        </li>
        <li class="flex cursor-pointer py-4 px-10">
          <div class="ml-4 mr-6">
            <img class="h-5" src="../assets/casual.png" alt />
          </div>
          <p>Casual</p>
        </li>
        <li class="flex cursor-pointer py-4 px-10">
          <div class="ml-4 mr-6">
            <img class="h-5" src="../assets/strategy.png" alt />
          </div>
          <p>Strategy</p>
        </li>
        <li class="flex cursor-pointer py-4 px-10">
          <div class="ml-4 mr-6">
            <img class="h-5" src="../assets/intellectual.png" alt />
          </div>
          <p>Intellectual</p>
        </li>
        <li class="flex cursor-pointer py-4 px-10">
          <div class="ml-4 mr-4">
            <img class="h-5" src="../assets/sport.png" alt />
          </div>
          <p>Sport</p>
        </li>
      </ul>
    </div>
    <div class="text-white mb-6 font-light px-8">
      <p>Recommended</p>
    </div>
    <div class="text-white mb-6 font-light px-8">
      <p>New</p>
    </div>
    <div class="text-white mb-6 font-light px-8">
      <p>Most Played</p>
    </div>
    <div class="px-8 py-6 mb-6 border-solid border-dark3 border-t border-b">
      <div class="flex items-center text-white">
        <img class="h-4 mr-4" src="../assets/mygames.png" alt="mygames" />
        <p>MY GAMES</p>
      </div>
    </div>

    <div class="flex justify-between px-8 mt-auto">
      <p class="text-font text-xs font-light select-none">Dark mode</p>
      <div
        @click="isActive = !isActive"
        :class="{darkMode:isActive}"
        class="border-solid border-toggle border rounded-full w-10 p-2px flex cursor-pointer"
      >
        <div class="bg-indigo-700 h-4 w-4 rounded-full"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: false,
      isNavOpen: false,
    };
  },
  methods: {}
};
</script>

<style>
.darkMode {
  justify-content: flex-end;
  background-color: #fff;
}
.toggleNav {
  display: none;
}
</style>


