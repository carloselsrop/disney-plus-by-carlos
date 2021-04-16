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
      <div class="flex flex-wrap w-8/12 justify-center">
        <User :img="'https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg'" :username="`Carlos`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/originals/13/38/56/133856009a021270fc2307e019eb7548.jpg'" :username="`Rodri`" :edit-profiles="editProfiles" />
        <User :img="'https://resizing.flixster.com/2SWqchwOqtMVrEXZO-uo5RjvRyI=/272x272/v1.czsxMDI3NTA4NztqOzE4ODA1OzIwNDg7MjcyOzI3Mg'" :username="`Steven`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/564x/ba/1c/c3/ba1cc3c72027f0c7b5c1095983edcc53.jpg'" :username="`Chicas`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/564x/35/ca/0e/35ca0edc099fb04581db95fa91d9d335.jpg'" :username="`July`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/564x/88/4b/7d/884b7ded2075bcdecfba6f8c8f2cff90.jpg'" :username="`Boris`" :edit-profiles="editProfiles" />
        <User :img="'https://i.pinimg.com/474x/f7/fc/7c/f7fc7c9b682c02736c3bced2cbc0c976.jpg'" :username="`Sebas`" :edit-profiles="editProfiles" />
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
