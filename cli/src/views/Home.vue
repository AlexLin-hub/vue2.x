<template>
  <div class="h-screen w-screen flex flex-col justify-center items-center">
    <h1 class="text-5xl mb-3">v-bind</h1>
    <div>
      <input
        v-model="value"
        class="
          border-2
          rounded-lg
          border-gray-800
          outline-none
          h-12
          py-3
          px-3
          focus:border-gray-700
          disabled:border-0
          disabled:text-gray-200
          disabled:placeholder:text-gray-200
        "
        type="text"
        placeholder="請輸入資料"
        autofocus
        v-bind:disabled="isDisabled"
      />
      <button
        class="
          ml-3
          text-white
          px-5
          py-3
          bg-gray-700
          rounded-lg
          shadow-md
          hover:bg-gray-600
        "
        v-on:click="turnOn()"
      >
        開啟
      </button>
    </div>
    <span class="text-lg mt-3">目前輸入的內容：{{ value || "尚未輸入" }}</span>
  </div>
</template>
<script>
export default {
  data() {
    return {
      value: "",
      isDisabled: true,
    };
  },
  methods: {
    turnOn() {
      this.isDisabled = false;
    },
  },
};
</script>
