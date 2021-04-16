<template>
  <div class="h-screen bg-gray-900">
    <!-- Navbar -->
    <div class="flex justify-between mx-8 py-4 items-center">
      <img class="w-16" src="@/static/disneyplus.png" alt="">
      <button v-if="editProfiles === false" class="px-6 bg-gray-500 py-2 font-semibold text-white rounded text-sm focus:outline-none" @click="editProfiles= true">
        EDITAR PERFILES
      </button>
      <button v-else class="py-2 px-4 bg-blue-500 rounded text-sm text-white font-semibold focus:outline-none" @click="editProfiles=false">
        Listo
      </button>
    </div>
    <!-- Pick a user -->
    <div class="flex pt-40 flex-col justify-center items-center">
      <div class="font-bold text-white text-3xl pb-10">
        ¿Quien eres?
      </div>
      <div class="flex space-x-12">
        <User :img="'https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg'" :username="`Carlos`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg'" :username="`Rodri`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg'" :username="`Steven`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg'" :username="`Chicas`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg'" :username="`Boris`" :edit-profiles="editProfiles" />
        <User username="Crear perfil" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    editProfiles: false
  })
}
</script>
