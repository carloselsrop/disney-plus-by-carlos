<template>
  <div class="w-full px-8 bg-gradient-to-b from-black to-gray-900 py-5 flex items-center">
    <!-- Disney plus logo -->
    <div class="pr-16">
      <img class="w-20" src="https://logodownload.org/wp-content/uploads/2020/11/disney-plus-logo-3.png" alt="">
    </div>
    <!-- Navigation Buttons -->
    <div>
      <div class="flex items-center space-x-14">
        <div class="flex items-center">
          <img class="w-3 h-3" src="https://freepikpsd.com/wp-content/uploads/2019/10/217-2171720_icon-white-house-home-icon-white-png.png" alt="">
          <div class="pl-2 text-sm font-semibold text-white">
            INICIO
          </div>
        </div>
        <div class="flex items-center">
          <img class="w-3 h-3" src="https://www.seekpng.com/png/full/920-9209972_magnifying-glass-png-white-search-icon-white-png.png" alt="">
          <div class="pl-2 text-sm font-semibold text-white">
            BÚSQUEDA
          </div>
        </div>
        <div class="flex items-center">
          <img class="w-3 h-3" src="@/static/plus.png" alt="">
          <div class="pl-2 text-sm font-semibold text-white">
            MI LISTA
          </div>
        </div>
        <div class="flex items-center">
          <img class="w-3 h-3" src="@/static/star.png" alt="">
          <div class="pl-2 text-sm font-semibold text-white">
            ORIGINALES
          </div>
        </div>
        <div class="flex items-center">
          <img class="w-3 h-3" src="@/static/film-reel.png" alt="">
          <div class="pl-2 text-sm font-semibold text-white">
            PELICULAS
          </div>
        </div>
        <div class="flex items-center">
          <img class="w-3 h-3" src="@/static/tv.png" alt="">
          <div class="pl-2 text-sm font-semibold text-white">
            SERIES
          </div>
        </div>
      </div>
    </div>
    <!-- Account -->
    <div class="flex items-center py-2 rounded-md pr-4 pt-4 bg-transparent z-50 absolute right-8 " @click="isOpen = ! isOpen">
      <div v-if="isOpen" class="flex flex-col absolute top-1 right-3 border-2 w-52 py-4 px-6 bg-gray-800 border-gray-500 z-30 rounded-md">
        <!-- Accounts -->
        <div class="space-y-4 pt-12">
          <div class="flex items-center">
            <img class="w-12 h-12 mr-2 rounded-full" src="https://i.pinimg.com/originals/25/27/59/252759aa916336f998ca11086015a16a.jpg" alt="">
            <div class="text-white">
              Carlos
            </div>
          </div>
          <div class="flex items-center">
            <img class="w-12 h-12 mr-2 rounded-full" src="https://i.pinimg.com/originals/13/38/56/133856009a021270fc2307e019eb7548.jpg" alt="">
            <div class="text-white">
              Rodri
            </div>
          </div>
          <div class="flex items-center">
            <img class="w-12 h-12 mr-2 rounded-full" src="https://resizing.flixster.com/2SWqchwOqtMVrEXZO-uo5RjvRyI=/272x272/v1.czsxMDI3NTA4NztqOzE4ODA1OzIwNDg7MjcyOzI3Mg" alt="">
            <div class="text-white">
              Steven
            </div>
          </div>
        </div>
        <!-- Options -->
        <div class="space-y-2 flex flex-col items-start pt-4">
          <button class="text-gray-200 text-sm focus:outline-none">
            Editar perfiles
          </button>
          <button class="text-gray-200 text-sm focus:outline-none">
            Ajustes de la aplicación
          </button>
          <button class="text-gray-200 text-sm focus:outline-none">
            Cuenta
          </button>
          <button class="text-gray-200 text-sm focus:outline-none">
            Ayuda
          </button>
          <NuxtLink to="/landing">
            <button class="text-gray-200 text-sm focus:outline-none">
              Cerrar sesión
            </button>
          </NuxtLink>
        </div>
      </div>
      <div class="text-white font-medium pl-4 pr-2 z-50">
        Steven
      </div>
      <img class="w-10 h-10 mr-4 rounded-full z-50" src="https://terrigen-cdn-dev.marvel.com/content/prod/1x/vision_1.jpg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    isOpen: false
  })
}
</script>
