<template>
  <div class="h-screen w-screen flex flex-col justify-center items-center">
    <h1 class="text-5xl mb-3">v-on.modifiers</h1>
    <div
      class="
        w-[300px]
        h-[300px]
        bg-gray-600
        rounded-xl
        flex flex-col
        items-center
        justify-center
        relative
        cursor-pointer
        shadow-md
      "
    >
      <p class="absolute top-2 text-white text-center">block01</p>
      <div
        class="
          w-[200px]
          h-[200px]
          bg-gray-300
          rounded-xl
          flex
          justify-center
          items-center
          cursor-pointer
          shadow-md
        "
      >
        <p class="text-black">block02</p>
      </div>
    </div>
  </div>
</template>