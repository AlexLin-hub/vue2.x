<template>
  <div class="h-screen w-screen flex flex-col justify-center items-center">
    <h1 class="text-5xl mb-3">v-model</h1>
    <input
      class="
        border-2
        rounded-lg
        border-gray-800
        focus:border-gray-700
        outline-none
        h-12
        py-3
        px-3
      "
      type="text"
      placeholder="請輸入資料"
      autofocus
    />
    <span class="text-lg mt-3">目前輸入的內容：{{ value || "尚未輸入" }}</span>
  </div>
</template>
<script>
export default {
  data() {
    return {
      value: "",
    };
  },
};
</script>
