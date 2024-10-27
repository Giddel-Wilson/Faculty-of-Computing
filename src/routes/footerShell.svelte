<script lang="ts">
  import {
    Facebook,
    Youtube,
    Twitter,
    Instagram,
    ArrowUp,
  } from "lucide-svelte";
</script>

<footer class="bg-green-600 text-white py-12">
  <div class="container mx-auto px-4">
    <div class="flex flex-wrap justify-between">
      <div class="w-full md:w-1/3 mb-8 md:mb-0">
        <h2 class="text-2xl font-bold mb-4">ABOUT US</h2>
        <p class="mb-4">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio
          consequatur ea dolorum quasi earum explicabo quae voluptates sit
          dignissimos placeat harum deserunt porro doloremque et, illum minus
          expedita maxime quisquam.
        </p>
        <div class="flex flex-col space-y-2">
          <span class="flex items-center">
            <svg
              class="w-4 h-4 mr-2 flex items-center"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
              ></path>
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
              ></path>
            </svg>
            Lorem ipsum dolor sit amet. At, molestias!
          </span>
          <span class="flex items-center">
            <svg
              class="w-4 h-4 mr-2"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
              ></path>
            </svg>
            nacosuniportexample@gmail.com
          </span>
          <span class="flex items-center">
            <svg
              class="w-4 h-4 mr-2"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M16 12a4 4 0 10-8 0 4 4 0 008 0zm0 0v1.5a2.5 2.5 0 005 0V12a9 9 0 10-9 9m4.5-1.206a8.959 8.959 0 01-4.5 1.207"
              ></path>
            </svg>
            @nacos_uniport
          </span>
        </div>
      </div>

      <div class="w-full md:w-1/3 mb-8 md:mb-0">
        <h2 class="text-2xl font-bold mb-4">QUICK LINK</h2>
        <ul class="space-y-2">
          <li><a href="/" class="hover:underline">Home</a></li>
          <li><a href="/login" class="hover:underline">Login</a></li>
          <li><a href="/about" class="hover:underline">About Us</a></li>
          <li><a href="/blog" class="hover:underline">Blog</a></li>
          <li><a href="/executives" class="hover:underline">Executives</a></li>
          <li><a href="/contact" class="hover:underline">Contact Us</a></li>
          <li><a href="/gallery" class="hover:underline">Gallery</a></li>
        </ul>
      </div>

      <div class="w-full md:w-1/3 hidden md:block">
        <h2 class="text-2xl font-bold mb-4">NEWS LATTER</h2>
        <p class="mb-4">
          Get NACOS OGITECH latest updates, news, and a lot more
        </p>
        <!-- Add newsletter form here if needed -->
      </div>
    </div>

    <div class="w-full md:w-1/3 md:hidden">
      <h2 class="text-2xl font-bold mb-4">NEWS LETTER</h2>
      <p class="mb-4">Get NACOS UNIPORT latest updates, news, and a lot more</p>
      <!-- Add newsletter form here if needed -->
    </div>
  </div>

  <div class="mt-12 border-t border-green-700 pt-8">
    <div
      class="container mx-auto px-4 flex flex-col md:flex-row justify-between items-center"
    >
      <p class="text-sm mb-4 md:mb-0 text-center md:text-left">
        Copyright © NACOS UNIPORT 2024/2025 . All Right Reserved.
      </p>
      <div class="flex space-x-4">
        <a href="./" class="text-white hover:text-green-300">
          <Facebook size={20} />
        </a>
        <a href="./" class="text-white hover:text-green-300">
          <Youtube size={20} />
        </a>
        <a href="./" class="text-white hover:text-green-300">
          <Twitter size={20} />
        </a>
        <a href="./" class="text-white hover:text-green-300">
          <Instagram size={20} />
        </a>
      </div>
    </div>
  </div>

  <!-- <button
        class="fixed bottom-10 opacity-80 hover:opacity-100 right-4 bg-green-600 text-white p-3 rounded-full shadow-lg hover:bg-transparent hover:text-green-600 hover:border-green-600 focus:outline-none focus:ring-2 focus:ring-green-400"
        on:click={() => window.scrollTo({ top: 0, behavior: 'smooth' })}
      >
        <ArrowUp size={24} />
      </button> -->
</footer>
