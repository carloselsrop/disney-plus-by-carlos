<template>
  <div class="ww-full h-screen bg-gray-900 pt-32">
    <!-- Email step -->
    <div v-if="step1 === false" class="flex flex-col items-center">
      <img class="w-32 mb-8" src="@/static/disneyplus.png" alt="">
      <div class="flex flex-col">
        <div class="font-semibold text-xl text-white pb-4">
          Inicia sesión con tu correo
        </div>
        <input id="" class="w-80 border-2 border-gray-600 rounded py-3 px-2 bg-gray-800 text-sm focus:border-gray-500 transition-colors duration-200 focus:outline-none" type="text" placeholder="Correo electrónico" name="">
        <button class="bg-blue-500 mt-8 py-3 px-2 text-center w-80 rounded font-semibold text-white focus:outline-none" @click="step1 = true">
          CONTINUAR
        </button>
        <div class="flex items-center mt-2">
          <div class="font-light text-sm text-gray-300">
            ¿Primera vez en Disney+?
          </div>
          <NuxtLink to="/landing">
            <button class="font-semibold text-sm text-white pl-1 focus:outline-none">
              Suscribirse
            </button>
          </NuxtLink>
        </div>
      </div>
    </div>
    <!-- Password step -->
    <div v-else class="flex flex-col items-center">
      <img class="w-32 mb-8" src="@/static/disneyplus.png" alt="">
      <div class="flex flex-col">
        <div class="font-semibold text-xl text-white pb-4">
          Escribe tu contraseña
        </div>
        <div class="relative">
          <svg xmlns="http://www.w3.org/2000/svg" class="absolute right-3 top-3 h-5 w-5 text-gray-200" viewBox="0 0 20 20" fill="currentColor">
            <path fill-rule="evenodd" d="M3.707 2.293a1 1 0 00-1.414 1.414l14 14a1 1 0 001.414-1.414l-1.473-1.473A10.014 10.014 0 0019.542 10C18.268 5.943 14.478 3 10 3a9.958 9.958 0 00-4.512 1.074l-1.78-1.781zm4.261 4.26l1.514 1.515a2.003 2.003 0 012.45 2.45l1.514 1.514a4 4 0 00-5.478-5.478z" clip-rule="evenodd" />
            <path d="M12.454 16.697L9.75 13.992a4 4 0 01-3.742-3.741L2.335 6.578A9.98 9.98 0 00.458 10c1.274 4.057 5.065 7 9.542 7 .847 0 1.669-.105 2.454-.303z" />
          </svg>
          <input id="" class="w-80 border-2 border-gray-600 rounded py-3 px-2 bg-gray-800 text-sm focus:border-gray-500 transition-colors duration-200 focus:outline-none" type="text" placeholder="Contraseña" name="">
        </div>

        <div class="text-sm text-gray-300 font-medium pt-1">
          Distingue mayúsculas y minúsculas.
        </div>
        <NuxtLink
          to="/"
        >
          <button
            class="bg-blue-500 mt-8 py-3 px-2 text-center w-80 rounded font-semibold text-white focus:outline-none"
          >
            INICIAR SESION
          </button>
        </NuxtLink>
        <div class="flex mt-2">
          <button class=" font-thin text-sm text-blue-400 focus:outline-none">
            ¿Olvidaste la contraseña?
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    step1: false
  })
}
</script>
