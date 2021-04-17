<template>
  <div class="bg-gray-900 w-full h-full">
    <!-- Navbar -->
    <Navbar />
    <!-- Slider -->
    <div class="py-6 mx-24">
      <Slider />
    </div>
    <!-- Categories -->
    <div class="mx-24 py-10 bg-red-500">
      <div class="w-full flex justify-between">
        <!-- Disney -->
        <div class="w-80 h-28 flex items-center justify-center rounded-lg shadow-xl py-20 bg-gray-800 border-2 border-gray-700 cursor-pointer">
          <div class="container bg-gray-800">
            <div class="text flex items-center justify-center">
              <img class="w-40" src="https://pngimg.com/uploads/walt_disney/walt_disney_PNG3.png" alt="">
            </div>
            <div class="img">
              <img class="h-40 rounded-md" src="https://media1.giphy.com/media/d8SMqAtm3D9bYfOtcs/giphy.gif" height="100%" width="100%" alt="">
            </div>
          </div>
        </div>
        <!-- Pixar -->
        <div class="w-80 h-28 flex items-center justify-center rounded-lg shadow-xl py-20 bg-gray-800 border-2 border-gray-700 cursor-pointer">
          <div class="container bg-gray-800">
            <div class="text flex items-center justify-center">
              <img class="w-60" src="https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/7F4E1A299763030A0A8527227AD2812C049CE3E02822F7EDEFCFA1CFB703DDA5/scale?width=600&aspectRatio=1.78&format=png" alt="">
            </div>
            <div class="img">
              <img class="h-40 rounded-md" src="https://media1.tenor.com/images/70eb5493160cd1108c37f5bcbafbb72a/tenor.gif?itemid=16128701" height="100%" width="100%" alt="">
            </div>
          </div>
        </div>
        <!-- Marvel -->
        <div class="w-80 h-28 flex items-center justify-center rounded-lg shadow-xl py-20 bg-gray-800 border-2 border-gray-700 cursor-pointer">
          <div class="container bg-gray-800">
            <div class="text flex items-center justify-center">
              <img class="w-40" src="https://logodownload.org/wp-content/uploads/2017/05/marvel-logo-4.png" alt="">
            </div>
            <div class="img">
              <img class="h-40 rounded-md" src="https://i.pinimg.com/originals/f2/d2/ee/f2d2ee07809be8f0139fb12071bb4d28.gif" height="100%" width="100%" alt="">
            </div>
          </div>
        </div>
        <!-- Star wars -->
        <div class="w-80 h-28 flex items-center justify-center rounded-lg shadow-xl py-20 bg-gray-800 border-2 border-gray-700 cursor-pointer">
          <div class="container bg-gray-800">
            <div class="text flex items-center justify-center">
              <img class="w-40" src="https://www.pngkit.com/png/full/0-6869_propel-star-wars-battle-drones-logo-star-wars.png" alt="">
            </div>
            <div class="img">
              <img class="h-40 rounded-md" src="https://media2.giphy.com/media/jUcEUcpxPMrFhR0f8f/giphy.gif" height="100%" width="100%" alt="">
            </div>
          </div>
        </div>
        <!-- National Geo -->
        <div class="w-80 h-28 flex items-center justify-center rounded-lg shadow-xl py-20 bg-gray-800 border-2 border-gray-700 cursor-pointer">
          <div class="container bg-gray-800">
            <div class="text flex items-center justify-center">
              <img class="w-60" src="https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/2EF24AA0A1E648E6D1A3B26491F516632137ED87AB22969D153316F8BD670FB5/scale?width=600&aspectRatio=1.78&format=png" alt="">
            </div>
            <div class="img">
              <img class="h-40 rounded-md" src="https://thumbs.gfycat.com/ConfusedCommonHeron-max-14mb.gif" height="100%" width="100%" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Recomendations -->
    <div class="mx-24 pb-10 mb-6">
      <div class="font-semibold text-white text-lg mb-4">
        Recomendaciones para ti
      </div>
      <div class="flex space-x-8">
        <MediaItem :url="'https://cannonball-cdn.bamgrid.com/assets/originals/mandalorian-season2.png'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/12BDB81547F6E32165F0A710618501A5E7848BA6C2222E0059D791384E2980E6/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/21734B29F0EACDD64FE8CD9BC5DFF519F55A0BA6A587751FB541AF367D65C30A/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/67903BA6F839B1D79525604B96EA477341928A134D18BDE3109CE21ED4019761/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/F6F8C5326039533D6D33164D07CB04D11212FAF484FA6D8E9230F966B5EA4624/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
      </div>
    </div>
    <!-- News on D+ -->
    <div class="mx-24 pb-10 mb-6">
      <div class="font-semibold text-white text-lg mb-4">
        Novedades en Disney +
      </div>
      <div class="flex space-x-8">
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/AB42129D458CA596E5431E2085BCDBB2336624B314EA23357A511BCF256F4DEA/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/CFA6BB9B1BE5E3D66981769809C93F70CC09250914E43EB4671C62ECEFECB513/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/B7AA43D258114894FD6B08F3DA71B760796F6E267976BBA783700F0AC8820A00/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/61F63CE3FE3A16ACB99792F54A643549BE1EEF71B310625C6F75D594D7FA2BDF/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://seriescienciaficcion.files.wordpress.com/2020/10/disney-plus-the-falcon-and-the-winter-soldier.jpg'" />
      </div>
    </div>
    <!-- Continue watching -->
    <div class="mx-24 pb-10">
      <div class="font-semibold text-white text-lg mb-4">
        Continuar viendo
      </div>
      <div class="flex space-x-8">
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/341AE85B6C1423B9042B5F2E786645EE551B9D546C3D263B220A4727617FD2B8/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/C0C1B5ABCCA0031878CC67872E9EC10143A88AAF2C81F5283F1CBBBAE572CBBD/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/090099C3B48344116520AFCDAD4C1EE19A349F4AD660E8E01C9C2728B2CABF21/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/6E428D528CA5B2508C55FE16EDBED8AD7E7A27435439D48584A15FD01B75F926/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
        <MediaItem :url="'https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/162CCE10190E261A552EABE15FD4B7C1464E51B73CB88052790A45EAC8073459/scale?width=1200&aspectRatio=1.78&format=jpeg'" />
      </div>
    </div>
    <!-- Footer -->
    <Footer />
  </div>
</template>

<style>
.container {
  width: 320px;
  height: 112px;
  position: relative
}
.container:hover .text {
  opacity: 0
}
.container:hover .img {
  opacity: 1
}
.text {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  text-align: center;
  left: 0;
  right: 0;
  opacity: 1;
  transition: opacity .3s linear;
}
.img {
  transition: opacity .3s linear;
  top: -24px;
  bottom: 120px;
  position: absolute;
  opacity: 0;
}
</style>
