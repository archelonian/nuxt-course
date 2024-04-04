<template>
  <div class="
    relative
    h-screen
    w-100
    bg-no-repeat
    bg-cover
    bg-bottom
    bg-[url('https://www.topgear.com/sites/default/files/2023/11/McLaren_750S_TheDrive-0847.jpg?w=1784&h=1004')]"

  >
    <div class="z-10 absolute w-full h-full flex justify-center items-center">
      <div class="text-center w-1/2">
        <h1 class="text-8xl font-serif mb-10 text-white">Find your drive.</h1>
        <CarSearchBar />
      </div>
    </div>
    <div class="z-1 absolute w-full h-full bg-black opacity-50"></div>
  </div>
</template>
