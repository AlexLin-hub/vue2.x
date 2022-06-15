<template>
  <div class="h-full rounded-lg px-3 py-2 shadow-lg relative">
    <button
      class="
        absolute
        bg-red-500
        text-white
        px-2
        py-1
        rounded-md
        right-4
        text-sm
      "
      v-on:click="$emit('onClick', '刪除')"
    >
      刪除
    </button>
    <h3 class="text-2xl font-bold text-gray-800">{{ user.name }}</h3>
    <h5 class="text-sm text-gray-400">{{ user.UID }}</h5>
    <h5 class="text-sm mt-3 text-gray-600">
      最後更新時間：{{ user.updateTime }}
    </h5>
  </div>
</template>
<script>
export default {
  props: {
    user: {
      type: Object,
      default: () => {},
    },
  },
};
</script>