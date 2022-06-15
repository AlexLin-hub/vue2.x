<template>
  <div class="flex flex-col justify-center items-center h-screen">
    <h1 class="text-5xl mb-3">v-if/v-show</h1>
    <div class="flex gap-5">
      <div
        v-if="isShow"
        class="
          w-[300px]
          h-[300px]
          bg-gray-700
          text-white
          flex
          justify-center
          items-center
          rounded-lg
        "
      >
        v-if
      </div>

      <div
        v-show="isShow"
        class="
          w-[300px]
          h-[300px]
          bg-gray-700
          text-white
          flex
          justify-center
          items-center
          rounded-lg
        "
      >
        v-show
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isShow: false,
    };
  },
};
</script>
