<template>
  <div style="background-image: url('https://cannonball-cdn.bamgrid.com/assets/originals/Mlp_Hero_Br_&_Rola_Desktop_v2.jpg')" class="h-screen w-full landing-back">
    <div>
      <NuxtLink to="/login">
        <button class="absolute right-6 top-6 text-white py-1 px-2 rounded-sm border-2 border-white focus:outline-none">
          INICIAR SESION
        </button>
      </NuxtLink>
    </div>
    <div class="h-full flex flex-col justify-center pl-16">
      <div>
        <img class="w-40 pb-8" src="@/static/disneyplus.png" alt="">
      </div>
      <div class="pb-8">
        <div class="text-white font-bold text-5xl pb-2">
          Las mejores historias,
        </div>
        <div class="text-white font-bold text-5xl">
          en un mismo lugar.
        </div>
      </div>
      <div class="flex pb-8">
        <!-- Month Price -->
        <div class="pr-12">
          <div class="flex items-end pb-2">
            <div class="text-white font-bold text-3xl">
              USD 5.99
            </div>
            <div class="text-gray-300">
              /mes*
            </div>
          </div>
          <div>
            <button class="px-20 text-xl bg-blue-500 text-white py-3 rounded font-light focus:outline-none">
              SUSCRIBETE AHORA
            </button>
          </div>
        </div>
        <!-- Year Price -->
        <div>
          <div class="flex items-end pb-2">
            <div class="text-white font-bold text-3xl">
              USD 59.99
            </div>
            <div class="text-gray-300">
              /año*
            </div>
          </div>
          <div>
            <button class="px-20 text-xl bg-blue-500 text-white py-3 rounded font-light focus:outline-none">
              SUSCRIBETE AHORA
            </button>
          </div>
        </div>
      </div>
      <div class="text-sm text-gray-300">
        *El precio podria variar en caso que el pago se realice en otras plataformas. Podrian aplicar cargos de terceros.
      </div>
    </div>
    <!-- Brands -->
    <div class="flex absolute bottom-6 left-16 items-center">
      <img class="w-24 h-10" src="https://pngimg.com/uploads/walt_disney/walt_disney_PNG3.png" alt="">
      <img class="w-4 mr-4 ml-8" src="@/static/plus.png" alt="">
      <img class="w-24 h-14" src="https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/7F4E1A299763030A0A8527227AD2812C049CE3E02822F7EDEFCFA1CFB703DDA5/scale?width=600&aspectRatio=1.78&format=png" alt="">
      <img class="w-4 mr-6 ml-2" src="@/static/plus.png" alt="">
      <img class="w-24 h-10" src="https://logodownload.org/wp-content/uploads/2017/05/marvel-logo-4.png" alt="">
      <img class="w-4 mr-6 ml-6" src="@/static/plus.png" alt="">
      <img class="w-24 h-10" src="https://www.pngkit.com/png/full/0-6869_propel-star-wars-battle-drones-logo-star-wars.png" alt="">
      <img class="w-4 mr-2 ml-8" src="@/static/plus.png" alt="">
      <img class="w-32 h-20" src="https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/2EF24AA0A1E648E6D1A3B26491F516632137ED87AB22969D153316F8BD670FB5/scale?width=600&aspectRatio=1.78&format=png" alt="">
    </div>
  </div>
</template>
