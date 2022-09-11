<template>
  <main class="flex items-center justify-center min-h-screen bg-slate-100">
    <section
      class="flex flex-col p-6 m-3 space-y-10 bg-white rounded-2xl shadow-2xl md:flex-row md:space-y-0 md:space-x-10 md:m-0 md:p-16"
    >
      <div>
        <img
          src="@/assets/image.webp"
          alt="blue bluetooth headphones"
          class="mx-auto hover:scale-105 duration-200 w-60"
        />
      </div>
      <div class="flex flex-col space-y-6">
        <div class="flex flex-col mb-4 space-y-3 text-center md:text-left">
          <div>
            <div
              class="inline-block px-3 py-1 text-white text-sm bg-black rounded-full"
            >
              Free Shipping
            </div>
          </div>
          <h1 class="max-w-sm text-2xl font-medium">
            Blue Bluetooth Gaming Headphones
          </h1>
          <div class="flex flex-col mb-4 space-y-3 text-center mb:text-left">
            <p class="line-through">$799</p>
            <p class="text-5xl font-bold">$599</p>
            <p class="text-small font-light text-gray-400">
              This offer is valid untill the stock lasts.
            </p>
          </div>
          <div class="group">
            <button
              class="w-full bg-blue-700 text-white border-b-8 border-b-blue-700 rounded-lg group-hover:border-t-8 group-hover:border-b-0 group-hover:bg-blue-700 group-hover:border-t-blue-700 group-hover:shadov-lg transition-all duration-200"
            >
              <div
                class="px-8 py-4 bg-blue-500 rounded-lg group-hover:bg-blue-700 duration-200"
              >
                Add To Cart
              </div>
            </button>
          </div>
          <div class="flex items-center space-x-3 group">
            <div
              class="w-3 h-3 bg-green-400 rounded-full group-hover:animate-ping"
            ></div>
            <p class="text-sm">50+ pcs. in stock</p>
          </div>
          <div
            class="flex flex-col space-y-4 md:space-y-0 md:space-x-4 md:flex-row"
          >
            <button
              class="flex items-center justify-center py-3 px-5 border-2 border-gray-300 rounded-lg shadow-sm hover:bg-opacity-30 hover:shadow-lg gover:-translate-y-0.5 transition-all duration-150 space-x-3"
            >
              <img
                src="@/assets/shopping-cart.png"
                alt="blue shopping cart icon"
                class="w-8"
              />
              <span>Add To Cart</span>
            </button>
            <button
              class="flex items-center justify-center py-3 px-5 border-2 border-gray-300 rounded-lg shadow-sm hover:bg-opacity-30 hover:shadow-lg gover:-translate-y-0.5 transition-all duration-150 space-x-3"
            >
              <img
                src="@/assets/balloons.png"
                alt="blue baloons shaped like a heart"
                class="w-8"
              />
              <span>Add To Wishlist</span>
            </button>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: "App",
};
</script>
