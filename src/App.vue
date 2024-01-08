<template>
  <div>
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
        autoplay
        loop
        muted
        class="min-h-[70vh] object-cover md:h-[90vh] w-screen"
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
        We've crafted three new speakers.The twist? They're all the same spaker.
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
        class="inner mx-4 md:mx-20 flex flex-col gap-5 md:gap-0 md:flex-row justify-between md:space-x-2"
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
      <div class="text-3xl md:text-4xl lg:text-5xl font font-[600] text-center">
        Superior craft since 1925
      </div>
      <button
        class="px-8 mt-8 text-black font-semibold border-2 border-black rounded-2xl bg-transparent transition duration-200 ease-in hover:bg-[#ffc356] hover:border-white py-1"
      >
        OurStory
      </button>
    </div>
  </div>
</template>
