<template>
  <div>
    <!-- pre-loader -->
    <transition name="curtains" mode="in-out">
      <div
        v-show="isLoading"
        key="loading"
        class="preloader flex flex-col gap-2"
      >
        <div
          class="text-3xl text-white font-bold tracking-tight cursor-pointer"
        >
          <!-- logo -->
          B<span class="text-lg">&</span>O
        </div>
        <div class="spinner"></div>
        <div class="text-white">Loading...</div>
      </div>
    </transition>

    <transition name="curtains" mode="out-in">
      <div v-show="!isLoading">
        <!-- top section nav+video+button -->
        <div class="nav mx-4 md:mx-0">
          <nav class="md:absolute font-sans" style="z-index: 10">
            <div
              class="flex p-3 px-8 md:p-5 md:px-10 md:text-white w-[98vw] justify-between"
            >
              <div class="lg:hidden font-bold text-2xl">&equiv;</div>
              <ul class="hidden lg:flex space-x-5 text-xs items-center">
                <div class="text-3xl font-bold tracking-tight cursor-pointer">
                  <!-- logo -->
                  B<span class="text-lg">&</span>O
                </div>
                <li
                  class="uppercase cursor-pointer hover:border-b-2 hover:border-b-yellow-400"
                >
                  Speakers
                </li>
                <li
                  class="uppercase cursor-pointer hover:border-b-2 hover:border-b-yellow-400"
                >
                  Headphones
                </li>
                <li
                  class="uppercase cursor-pointer hover:border-b-2 hover:border-b-yellow-400"
                >
                  Televisions
                </li>
                <li
                  class="uppercase cursor-pointer hover:border-b-2 hover:border-b-yellow-400"
                >
                  Soundbars
                </li>
                <li
                  class="uppercase cursor-pointer hover:border-b-2 hover:border-b-yellow-400"
                >
                  World of b&o
                </li>
                <li
                  class="uppercase cursor-pointer hover:border-b-2 hover:border-b-yellow-400"
                >
                  support
                </li>
              </ul>

              <div
                class="lg:hidden text-3xl font-bold tracking-tight cursor-pointer"
              >
                <!-- logo -->
                B<span class="text-lg">&</span>O
              </div>

              <!-- Icons -->
              <div class="flex space-x-6 items-center">
                <div>
                  <!-- user icon -->
                  <i class="fa-regular fa-user cursor-pointer"></i>
                </div>
                <div>
                  <!-- location icon  -->
                  <i class="fa-solid fa-location-dot cursor-pointer"></i>
                </div>
                <div>
                  <!-- Cart icon -->
                  <i class="fa-brands fa-opencart cursor-pointer"></i>
                </div>
              </div>
            </div>
          </nav>
          <video
            playsinline
            autoplay
            loop
            muted
            class="min-h-[70vh] object-cover md:h-[90vh] w-screen bg-white"
            style="z-index: -10"
          >
            <source src="./assets/video/Beolab-8-video-home.mp4" />
          </video>
        </div>
        <div
          class="flex flex-col items-center md:items-start md:pl-20 -mt-[15rem] md:-mt-[17rem] mx-4 md:mx-0"
        >
          <div class="font-bold text-7xl text-white" style="z-index: 10">
            Beolab 8
          </div>
          <div
            class="text-white w-[80vw] text-center md:text-left md:w-[28vw] lg:w-[23vw] my-5 font-semibold"
            style="z-index: 10"
          >
            We've crafted three new speakers.The twist? They're all the same
            spaker.
          </div>

          <button
            class="bg-[#ffc356] rounded-3xl px-8 py-2 text-[#30291d] font-bold hover:bg-[#f5ce85]"
            style="z-index: 10"
          >
            Discover more
          </button>
        </div>

        <!-- 4 cards -->
        <div
          class="main md:mt-[2.5rem] lg:mt-[4rem] py-6 md:h-96 flex flex-col justify-center mt-[4rem]"
        >
          <div
            class="inner mx-4 md:mx-20 flex flex-col gap-5 md:gap-0 md:flex-row justify-between md:space-x-2 xl:mx-[15rem] 2xl:mx-[40rem]"
          >
            <div
              class="flex flex-col items-center md:w-[15.5rem] hover:brightness-90 cursor-pointer"
            >
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/7zxzNPdEmgcwLMu84yKyp5/94070bef5f1a26b7ce7edd814b066f2f/Beosound_A5_-_Rich_Media_-_Closeup.png?q=90&fm=webp&w=480&h=480&fit=fill"
                alt=""
                class="hidden md:flex brightness-75 transform hover:scale-110 transition-transform duration-300 ease-in-out"
                style="z-index: -2"
              />
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/7zxzNPdEmgcwLMu84yKyp5/94070bef5f1a26b7ce7edd814b066f2f/Beosound_A5_-_Rich_Media_-_Closeup.png?q=90&fm=webp&w=480&h=240&fit=fill"
                alt=""
                class="md:hidden w-[100%] h-auto"
              />
              <div
                class="-mt-[3rem] text-white font-semibold text-2xl tracking-wide"
              >
                Speakers
              </div>
            </div>
            <div
              class="flex flex-col items-center md:w-[15.5rem] hover:brightness-90 cursor-pointer"
            >
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/rKK6o7IhiJ4ZKdMHByaEh/1bac9875ec112215d576f5f97c208bff/headphone2.png?q=90&fm=webp&w=480&h=480&fit=fill"
                alt=""
                class="hidden md:flex brightness-75 transform hover:scale-110 transition-transform duration-300 ease-in-out"
                style="z-index: -2"
              />
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/rKK6o7IhiJ4ZKdMHByaEh/1bac9875ec112215d576f5f97c208bff/headphone2.png?q=90&fm=webp&w=480&h=240&fit=fill"
                alt=""
                class="md:hidden w-[100%] h-auto"
              />
              <div
                class="-mt-[3rem] text-white font-semibold text-2xl tracking-wide"
              >
                Headphones
              </div>
            </div>
            <div
              class="flex flex-col items-center md:w-[15.5rem] hover:brightness-90 cursor-pointer"
            >
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/3VKLdZqyWi2sYk0WleFLOK/967677d067aace59a0dab10fbc9fb3de/TV.png?q=90&fm=webp&w=480&h=480&fit=fill"
                alt=""
                class="hidden md:flex brightness-75 transform hover:scale-110 transition-transform duration-300 ease-in-out"
                style="z-index: -2"
              />
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/3VKLdZqyWi2sYk0WleFLOK/967677d067aace59a0dab10fbc9fb3de/TV.png?q=90&fm=webp&w=480&h=240&fit=fill"
                alt=""
                class="md:hidden w-[100%] h-auto"
              />
              <div
                class="-mt-[3rem] text-white font-semibold text-2xl tracking-wide"
              >
                Televisions
              </div>
            </div>
            <div
              class="flex flex-col items-center md:w-[15.5rem] hover:brightness-90 cursor-pointer"
            >
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/4vXH4MKTOsMgJr4uiyulP8/49c6fcf4841855100e47b599580c4a5a/Soundbars.png?q=90&fm=webp&w=480&h=480&fit=fill"
                alt=""
                class="hidden md:flex brightness-75 transform hover:scale-110 transition-transform duration-300 ease-in-out"
                style="z-index: -2"
              />
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/4vXH4MKTOsMgJr4uiyulP8/49c6fcf4841855100e47b599580c4a5a/Soundbars.png?q=90&fm=webp&w=480&h=240&fit=fill"
                alt=""
                class="md:hidden w-[100%] h-auto"
              />
              <div
                class="-mt-[3rem] text-white font-semibold text-2xl tracking-wide"
              >
                Soundbars
              </div>
            </div>
          </div>
        </div>

        <!--Our Story heading -->
        <div class="flex flex-col items-center py-20 gap-5">
          <div class="font-semibold text-slate-600 text-lg">BANG & OLUFSEN</div>
          <div
            class="text-3xl md:text-4xl lg:text-5xl font font-[600] text-center"
          >
            Superior craft since 1925
          </div>
          <button
            class="px-8 mt-8 text-black font-semibold border-2 border-black rounded-2xl bg-transparent transition duration-200 ease-in hover:bg-[#ffc356] hover:border-white py-1"
          >
            OurStory
          </button>
        </div>

        <!-- cutting/crafting video -->

        <video
          playsinline
          autoplay
          loop
          muted
          src="//videos.ctfassets.net/8cd2csgvqd3m/sxXAwBnfBnfImWlDMXsaH/b57c7e3cf06623bf5883b59468492a1f/CraftMatters_Alu.mp4"
          class="min-h-[70vh] object-cover md:h-full w-screen p-10 md:p-14 lg:p-20 bg-white"
        ></video>

        <!-- picture button // connected speakers area -->
        <div
          style="
            background-image: url(https://images.ctfassets.net/8cd2csgvqd3m/5dU3DUbSEonydEHBTOIo0U/fd0bf1cdf5ef840b786e1c05ac17ef36/LS_2020-06_BV-Harmony-65_Silver-Alu-Oak___BL18_Silver-Alu-Oak___BL19_Black-Brass-Straight_w_light-square.jpg?q=90&w=2048&fit=fill&fm=webp);
          "
          class="h-[90vh] md:h-[75vh] bg-cover bg-center bg-no-repeat flex items-center"
        >
          <div
            class="text-white backdrop-brightness-[0.7] w-[80vw] md:w-[44vw] h-min ml-16 space-y-6 p-6"
          >
            <div class="text-5xl">Connected Speakers</div>
            <div>
              No cables, no fuss. Connect speakers quickly and easily through
              WiFi, and be connected everywhere. Control the whole experience
              from the palm of your hand: play what you want, the way you want.
            </div>
            <div
              class="px-5 mt-8 font-semibold outline outline-white rounded-2xl bg-transparent transition duration-200 ease-in hover:bg-[#ffc356] hover:outline-none py-1 inline-block"
            >
              <button>Connected Speakers</button>
            </div>
          </div>
        </div>

        <!-- Find Store -->
        <div
          class="main flex justify-center items-center md:h-[75vh] bg-[#f5f4f3]"
        >
          <div
            class="inner flex flex-col md:flex-row h-auto md:h-[50vh] mt-10 md:mt-0 mb-16 md:mb-0 bg-white overflow-hidden mx-3 md:mx-10"
          >
            <div class="mx-auto">
              <img
                src="https://images.ctfassets.net/8cd2csgvqd3m/2C4PDfprsTL0Z2UEZtvpvg/793a067fe33a8086e00f8cc6396586ca/Underc_111223-19.jpg?q=85&fm=webp&w=720&h=405&fit=fill"
                alt=""
                class="transform hover:scale-110 transition-transform duration-300 ease-in-out min-h-full"
              />
            </div>

            <div
              class="subInner flex flex-col items-start md:justify-center md:items-center space-y-5 px-5 py-5 md:py-0 md:px-20 min-w-[50vw] 0"
            >
              <div class="md:text-center text-lg font-semibold">
                UP CLOSE AND PERSONAL
              </div>
              <div class="md:text-center text-3xl font-bold">
                Experience in store
              </div>
              <div class="md:text-center text-sm font-[500] md:w-[28vw]">
                Come by one of our stores to hear, see and feel Bang & Olufsen
                yourself.
              </div>
              <button
                class="px-8 mt-8 text-black font-semibold border-2 border-black rounded-2xl bg-transparent transition duration-200 ease-in hover:bg-[#ffc356] hover:border-white py-1"
              >
                Find store
              </button>
            </div>
          </div>
        </div>

        <!-- Footer -->
        <div class="main h-[70vh] bg-[#191817] text-white flex flex-col gap-10">
          <div
            class="innerMain flex flex-col md:flex-row gap-16 md:gap-0 lg:gap-10 h-auto md:mx-[7rem] mt-16 md:mt-32 lg:mt-52"
          >
            <div
              class="subInner uppercase flex flex-col md:flex-row flex-wrap md:w-[80rem] items-center text-xl gap-5 md:gap-10 lg:gap-20 font-semibold"
            >
              <div class="options cursor-pointer">
                Customer care<span class="mx-5">&#8964;</span>
              </div>
              <div class="options cursor-pointer">
                our policies<span class="mx-5">&#8964;</span>
              </div>
              <div class="options cursor-pointer">
                our company<span class="mx-5">&#8964;</span>
              </div>
              <div class="options cursor-pointer">
                social links<span class="mx-5">&#8964;</span>
              </div>
              <div class="options cursor-pointer">
                download our apps<span class="mx-5">&#8964;</span>
              </div>
            </div>
            <div class="subInner text-2xl font-semibold text-center">
              Lang: International 🌏
            </div>
          </div>
          <div
            class="innerMain text-center md:pl-28 text-sm md:text-start md:mt-9 font-[400]"
          >
            © Bang & Olufsen 2024
          </div>
        </div>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isLoading: true,
    };
  },
  mounted() {
    setTimeout(() => {
      this.isLoading = false;
    }, 2000);
  },
};
</script>

<style scoped>
.preloader {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
}

.spinner {
  border: 4px solid #f3f3f3;
  border-top: 4px solid #db3434;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  animation: spin 1.2s linear infinite;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

.curtains-enter-active,
.curtains-leave-active {
  transition: opacity 1s, transform 1s;
}

.curtains-enter,
.curtains-leave-to {
  opacity: 0;
  transform:  scaleX(-1);
  
}
</style>
