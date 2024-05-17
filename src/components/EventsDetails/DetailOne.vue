<template>
  <nav class="text-black">
    <div data-aos="zoom-in" class="container flex flex-col items-start p-2">
      <button class="bg-gray-200 text-gray-500 py-1 px-3 rounded-full">Événements physiques</button>
      <h1 class="text-xl sm:text-xl font-bold ml-1 mt-2">
        lancement officiel : Congo Telema Event 2024
      </h1>
    </div>
    <hr class="border-t-2 border-gray-300" />
    <p class="text-lg text-gray-800 text-justify">
      Je suis la description de cet événement géré par cette application merveilleuse.
      <a href="#" class="text-blue-500 hover:underline">Lire plus</a>
    </p>
    <div class="flex items-start space-x-2">
      <span
        class="cursor-pointer rounded-lg border-gray-900/5 bg-black p-2 text-white transition-colors hover:border-gray-900/10 hover:bg-gray-900/10 hover:!opacity-100 group-hover:opacity-70"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-6 h-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M14.25 6.087c0-.355.186-.676.401-.959.221-.29.349-.634.349-1.003 0-1.036-1.007-1.875-2.25-1.875s-2.25.84-2.25 1.875c0 .369.128.713.349 1.003.215.283.401.604.401.959v0a.64.64 0 0 1-.657.643 48.39 48.39 0 0 1-4.163-.3c.186 1.613.293 3.25.315 4.907a.656.656 0 0 1-.658.663v0c-.355 0-.676-.186-.959-.401a1.647 1.647 0 0 0-1.003-.349c-1.036 0-1.875 1.007-1.875 2.25s.84 2.25 1.875 2.25c.369 0 .713-.128 1.003-.349.283-.215.604-.401.959-.401v0c.31 0 .555.26.532.57a48.039 48.039 0 0 1-.642 5.056c1.518.19 3.058.309 4.616.354a.64.64 0 0 0 .657-.643v0c0-.355-.186-.676-.401-.959a1.647 1.647 0 0 1-.349-1.003c0-1.035 1.008-1.875 2.25-1.875 1.243 0 2.25.84 2.25 1.875 0 .369-.128.713-.349 1.003-.215.283-.4.604-.4.959v0c0 .333.277.599.61.58a48.1 48.1 0 0 0 5.427-.63 48.05 48.05 0 0 0 .582-4.717.532.532 0 0 0-.533-.57v0c-.355 0-.676.186-.959.401-.29.221-.634.349-1.003.349-1.035 0-1.875-1.007-1.875-2.25s.84-2.25 1.875-2.25c.37 0 .713.128 1.003.349.283.215.604.401.96.401v0a.656.656 0 0 0 .658-.663 48.422 48.422 0 0 0-.37-5.36c-1.886.342-3.81.574-5.766.689a.578.578 0 0 1-.61-.58v0Z"
          />
        </svg>
      </span>

      <div class="flex flex-col space-y-1">
        <span class="text-gray-400">Powered/Hosted by</span>
        <span class="text-black-600 font-bold">Sponsor/Host name</span>
      </div>
    </div>
    <div class="my-4 flex -space-x-2 overflow-hidden">
      <img
        class="inline-block h-10 w-10 rounded-full ring-2 ring-white"
        src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
        alt=""
      />
      <img
        class="inline-block h-10 w-10 rounded-full ring-2 ring-white"
        src="https://images.unsplash.com/photo-1550525811-e5869dd03032?ixlib=rb-1.2.1&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
        alt=""
      />
      <img
        class="inline-block h-10 w-10 rounded-full ring-2 ring-white"
        src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=256&h=256&q=80"
        alt=""
      />

      <p class="inline-block h-10 w-10 bg-white rounded-full ring-1 ring-black border">
        <span class="font-bold text-xl">24</span>
      </p>
    </div>
  </nav>
</template>
<script>
import { defineComponent } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

export default defineComponent({
  mounted() {
    AOS.init()
  }
})
</script>