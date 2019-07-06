<template>
  <div class="bg-dark flex border-solid border-dark3 border-b">
    <div class="bg-dark2 flex items-center w-1/5 px-4 py-2">
      <img class="h-16" src="../assets/logo.png" alt="logo" />
      <p class="text-white mr-2 text-xs">UPROAR</p>
      <div class="bg-light px-3 text-white rounded-sm text-xs">
        <p>beta</p>
      </div>
    </div>
    <div class="flex container mx-auto justify-between w-4/5 py-2">
      <div class="flex">
        <nav class="ont-light py-4">
          <a class="px-4 text-sm inline-block text-gray-500" href>FAQ</a>
          <a class="px-4 text-sm inline-block text-gray-500" href>About</a>
          <a
            class="px-4 text-sm inline-block text-gray-500 border-solid border-r border-gray-600"
            href
          >Support</a>
        </nav>
        <div class="flex items-center ml-4">
          <img src="@/assets/flag.png" class="mr-2" alt />
          <select class="text-sm bg-transparent text-gray-200" name id>
            <option value>Eng</option>
            <option value>Tr</option>
          </select>
        </div>
      </div>
      <div class="flex items-center">
        <div class="bg-light flex items-center px-2 ml-6 rounded-lg">
          <div class="rounded-lg mr-3 w-12">
            <img class="h-auto w-auto" src="../assets/coin.png" alt />
          </div>
          <div class="mr-2 text-white">
            <p class="text-sm">650</p>
          </div>
          <div class="font-bold text-white text-sm">
            <p>+</p>
          </div>
        </div>
        <div class="bg-light flex items-center px-2 ml-6 rounded-lg">
          <div class="rounded-lg mr-3 w-12">
            <img class="h-auto w-auto" src="../assets/energy.png" alt />
          </div>
          <div class="mr-2 text-white">
            <p class="text-sm">1200</p>
          </div>
          <div class="text-gray-500 text-sm">+5/hour</div>
        </div>
        <div class="flex items-center ml-6">
          <div class="mr-4 h-12 w-12">
            <img class="w-auto h-auto" src="../assets/profil.png" alt />
          </div>
          <div class="my-auto">
            <p class="text-white font-semibold">Jeremy Manning</p>
            <div class="relative">
              <p class="text-green-400 font-semibold ml-5">Online</p>
              <div class="dot"></div>
            </div>
          </div>
          <div class="-mt-5 px-3 rounded-lg ml-4 bg-button text-white">
            <p class="text-sm">PRO</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>