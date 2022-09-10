<template>
  <main class="flex items-center justify-center h-screen bg-zinc-700">
    <section class="bg-zinc-800 p-2 mx-6 rounded-2xl">
      <div class="flex flex-col md:flex-row rounded-l-xl">
        <img
          src="@/assets/gnocchi.jpg"
          alt=""
          class="object-fit rounded-xl h-80 md:h-64 md:rounded-l-xl md:rounded-r-none transform hover:scale-105 hover:rounded-xl duration-200"
        />
        <div class="p-6 md:p-12">
          <h2
            class="font-serif text-xl font-medium text-center text-slate-200 md:text-left"
          >
            Get tasty vegetarian recepies to your inbox
          </h2>
          <p
            class="max-w-s my-4 text-xs leading-5 tracking-wide text-center text-slate-300 md:text-left"
          >
            Surprise your loved-ones with a nice meal. Sign up for easy daily
            recepies.
          </p>
          <div
            class="flex flex-col md:flex-row mt-5 space-y-4 md:space-y-0 md:space-x-3"
          >
            <input
              type="email"
              placeholder="enter your email here"
              class="p-2 px-4 text-center text-slate-300 bg-zinc-800 border border-zinc-600 placeholder:text-xs placeholder:text-center md:text-left placeholder:md:text-left focus:outline-none rounded-sm"
            />
            <button
              class="px-5 py-3 text-xs rounded-md text-zinc-800 bg-lime-500 hover:bg-lime-700 hover:text-slate-300 duration-200"
            >
              Subscribe
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
