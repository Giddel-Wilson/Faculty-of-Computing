<script>
  import {
    Facebook,
    Youtube,
    Twitter,
    Instagram,
    ChevronUpIcon,
  } from "lucide-svelte";
  import { onMount } from "svelte";

  let isScrolled = false;

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 50;
    };

    window.addEventListener("scroll", handleScroll);

    return () => {
      window.removeEventListener("scroll", handleScroll);
    };
  });
</script>

<footer class="bg-green-600 text-white py-12">
  <div class="mt-12 border-t border-green-700 pt-8">
    <p class="text-sm mb-4 md:mb-0 text-center md:text-left">
      Copyright © NACOS UNIPORT 2024/2025 . All Right Reserved.
    </p>
  </div>

  <button
        class="fixed bottom-10 hover:opacity-100 right-4 bg-green-500 text-white p-3 rounded-full shadow-lg focus:outline-none focus:ring-2 focus:ring-green-400 focus:bg-transparent focus:text-green-500"
        class:hidden={!isScrolled}
        on:click={() => window.scrollTo({ top: 0, behavior: 'smooth' })}
      >
        <ChevronUpIcon size={24} class="animate-bounce" />
      </button>
</footer>
