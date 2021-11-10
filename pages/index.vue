<template>
  <div class="min-h-screen">
    <div
      class="
        sticky
        top-0
        z-50
        inset-0
        bg-gray-900
        p-2
        flex
        items-center
        justify-between
      "
    >
      <img
        class="w-12"
        src="https://res.cloudinary.com/mctony17/image/upload/v1636111973/zubiks/Logopit.png"
        alt="logo"
      />
      <div class="flex items-center space-x-4">
        <n-link
          class="text-white md:text-lg font-medium tracking-wide"
          to="#about"
          >ABOUT US</n-link
        >
        <n-link
          class="text-white md:text-lg font-medium tracking-wide"
          to="#catalogue"
          >CATALOGUE</n-link
        >
        <n-link
          class="text-white md:text-lg font-medium tracking-wide"
          to="#contact"
          >CONTACT</n-link
        >
      </div>
    </div>
    <!-- <div
    class="w-full h-full bg-no-repeat bg-cover bg-center bg-fixed"
    style="background-image: url('https://res.cloudinary.com/mctony17/image/upload/v1636214505/zubiks/banner4.webp');"
    > -->
    <div
      class="w-full h-screen bg-fixed bg-cover bg-center"
      :style="{
        backgroundImage: `url(${require('@/static/bgimage/banner3.webp')})`,
      }"
    >
      <div class="h-screen flex flex-col items-center justify-center">
        <section
          class="
            bg-black
            opacity-75
            pt-2
            pb-4
            px-12
            rounded-lg
            text-center text-gray-400
            font-semibold
            text-2xl
            tracking-widest
          "
        >
          <h3 class="welcomefont">WELCOME TO</h3>
          <h1 class="donfont text-blue-600 font-bold text-4xl">DON-ZUBIKS</h1>
          <h3 class="welcomefont">METAL LTD.</h3>
          <div class="text-base mt-6 space-x-2">
            <button
              class="
                hover:text-blue-600
                font-medium
                tracking-wider
                py-2
                px-4
                rounded-lg
                border-2
                focus:outline-none
              "
            >
              <a href="#about">ABOUT US</a>
            </button>
            <button
              class="
                bg-blue-500
                hover:bg-blue-700
                text-white
                font-medium
                tracking-wider
                py-2
                px-4
                rounded-lg
                border-4 border-blue-500
                focus:outline-none
              "
            >
              <a href="#catalogue">CATALOGUE</a>
            </button>
          </div>
        </section>
      </div>
    </div>

    <!-- Body -->
    <div class="pt-8 space-y-6">
      <!-- About Us -->
      <div id="about" class="px-3 max-w-5xl mx-auto">
        <div
          class="
            rounded-lg
            border
            overflow-hidden
            shadow-lg
            md:flex md:items-center md:justify-center md:space-x-6
          "
        >
          <img
            class="w-full"
            src="https://res.cloudinary.com/mctony17/image/upload/v1636065327/zubiks/ceo.jpg"
            alt="CEO"
          />
          <div class="py-6 px-4">
            <h2 class="font-bold text-blue-600 tracking-widest text-2xl">
              ABOUT US
            </h2>
            <div class="h-1 w-20 bg-blue-300"></div>
            <div class="mt-4 text-gray-700 text-lg space-y-4">
              <p>
                My name is Ani Godswill Azubuike and I am the Chief Executive
                Officer, CEO, of Don-Zubiks Metal Ltd.
              </p>
              <p>
                Don-Zubiks Metal Ltd is a registered company that deals in all
                kinds of building materials such as: Wrought Iron, Stainles
                Handrails, Crytal Handrails, Aluminium Rails and Accessories,
                Foreign Doors, Water Collector, PVC Ceilling, Suspended, Tiles &
                Marble, Roofing Sheets, Glass Block and Fencing Wires.
              </p>
              <p>At Don-Zubiks Metal Ltd, our priority is your satisfaction</p>
            </div>
          </div>
        </div>
      </div>
      <!-- Catalogue -->
      <div id="catalogue" class="bg-gray-200">
        <div class="px-3 py-6 max-w-5xl mx-auto">
          <h2 class="mt-8 font-bold text-blue-600 tracking-widest text-2xl">
            CATALOGUE
          </h2>
          <div class="h-1 w-20 bg-blue-300"></div>
          <h3 class="py-4 italic text-gray-600 text-lg tracking-wide">
            See our creative designs below and we are creating more for your satisfaction...
          </h3>
          <!-- cards -->
          <div class="mt-12 mb-8 grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
            <div
              v-for="image in cloudinaryImages"
              :key="image.id"
              class="bg-white border rounded-lg shadow-xl overflow-hidden"
            >
              <img class="w-full" :src="image" alt="metal work images" />
              <!-- <div class="px-6 py-4">
                <div class="font-bold text-xl mb-2">The Coldest Sunset</div>
              </div> -->
            </div>
          </div>
        </div>
      </div>
      <!-- Footer -->
      <div id="contact" class="bg-gray-800 py-8 text-gray-600">
        <img
          class="w-20 h-20"
          src="https://res.cloudinary.com/mctony17/image/upload/v1636111973/zubiks/Logopit.png"
          alt="logo"
        />
        <div class="px-4">
          <h1 class="donfont font-bold tracking-wider text-2xl text-gray-500">
            DON-ZUBIKS METAL LTD
          </h1>
          <br />
          <hr />
          <div class="my-6 tracking-wide">
            <h3 class="text-xl md:text-center font-bold text-gray-500">
              CONTACT:
            </h3>
            <div class="space-y-6 sm:grid sm:grid-cols-2 lg:grid-cols-4">
              <!-- Head office -->
              <div class="mt-4 text-base">
                <h3 class="font-bold text-gray-500">HEAD OFFICE</h3>
                <p>No. OGB347 / OGB348</p>
                <p>Importer Zone Opp. Building Materials Int'l Market</p>
                <p>Ogbunike /Ogidi, Anambra State</p>
              </div>
              <!-- Contact office -->
              <div class="text-base">
                <h3 class="font-bold text-gray-500">CONTACT OFFICE</h3>
                <p>Zone 2, G85</p>
                <p>Main Line, Building Materials Int'l Market</p>
                <p>Ogbunike /Ogidi, Anambra State</p>
              </div>

              <!-- Workshop -->
              <div class="text-base">
                <h3 class="font-bold text-gray-500">WORKSHOP</h3>
                <p>No. 1 Ugwunwasike Road</p>
                <p>Opp. Importers Zone</p>
                <p>Ogbunike /Ogidi, Anambra State</p>
              </div>
              <!-- Tell -->
              <div class="text-base">
                <h3 class="font-bold text-gray-500">
                  BUSINESS TELLEPHONE LINES
                </h3>
                <p>08064181850</p>
                <p>08039941094</p>
                <p>09042402397</p>
              </div>
            </div>
          </div>
        </div>
        <hr />
        <div class="px-2">
          <h3 class="tracking-wider text-sm text-center mt-8 italic">
            Software developer contact: 08063856120 / matgold17@gmail.com
          </h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      images: [
        "zubiks/z1",
        "zubiks/z2",
        "zubiks/z3",
        "zubiks/z4",
        "zubiks/z5",
        "zubiks/z6",       
        "zubiks/z8",       
        "zubiks/z10",
        "zubiks/z11",
        "zubiks/z12",
        "zubiks/z13",
        "zubiks/z14",
        "zubiks/z15",
        "zubiks/z16",
        "zubiks/z17",
        "zubiks/z18",
        "zubiks/z19",
        "zubiks/z20",
        "zubiks/z21",
        "zubiks/z22",
        "zubiks/z23",
        "zubiks/z24",
        "zubiks/z25",
        "zubiks/z26",
        "zubiks/z27",
        "zubiks/z28",
        "zubiks/z31",
        "zubiks/z33",
        "zubiks/z34",
        "zubiks/z35",
        "zubiks/z36",
        "zubiks/z38",
        "zubiks/z41",
        "zubiks/z42",
        "zubiks/z43",
        "zubiks/z44",
      ],
    };
  },
  computed: {
    cloudinaryImages() {
      return this.images.map((image) => {
        return this.$cloudinary.image.url(image);
      });
    },
  },
};
</script>

<style>
h3.welcomefont {
  font-family: Dekko, sans-serif;
}

h1.donfont {
  font-family: Limelight, sans-serif;
}
</style>
