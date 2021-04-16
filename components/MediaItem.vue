<template>
  <div class="w-80 h-40 shadow-2xl transform transition-all border-2 rounded-lg border-gray-900 duration-500 hover:scale-110 hover:border-white cursor-pointer">
    <img class="w-full h-full rounded-md" :src="url" alt="">
  </div>
</template>

<script>
export default {
  props: {
    url: {
      type: String,
      required: true
    }
  }
}
</script>
