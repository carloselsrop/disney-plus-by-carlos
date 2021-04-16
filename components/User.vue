<template>
  <div class="relative">
    <img v-if="img" class="w-40 h-40 rounded-full mb-2 cursor-pointer" :src="img" alt="">
    <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-40 text-white mb-2 cursor-pointer bg-gray-700 rounded-full w-40" viewBox="0 0 20 20" fill="currentColor">
      <path fill-rule="evenodd" d="M10 5a1 1 0 011 1v3h3a1 1 0 110 2h-3v3a1 1 0 11-2 0v-3H6a1 1 0 110-2h3V6a1 1 0 011-1z" clip-rule="evenodd" />
    </svg>
    <div class="font-bold text-2xl text-white text-center cursor-pointer">
      {{ username }}
    </div>
    <button v-if="editProfiles" class="absolute bottom-12 right-2 bg-white rounded-full p-2">
      <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
        <path d="M13.586 3.586a2 2 0 112.828 2.828l-.793.793-2.828-2.828.793-.793zM11.379 5.793L3 14.172V17h2.828l8.38-8.379-2.83-2.828z" />
      </svg>
    </button>
  </div>
</template>

<script>
export default {
  props: {
    img: {
      type: String,
      default: ''
    },
    username: {
      type: String,
      required: true
    },
    editProfiles: {
      type: Boolean,
      default: false
    }
  }
}
</script>
