<script lang="ts">
    export let year: string;
    export let name: string;
    export let image: string;
    </script>
    
    <div class="flex items-start mb-8">
      <div class="w-1/4 text-right pr-4">
        <span class="text-lg font-bold">{year}</span>
      </div>
      <div class="w-1/4 flex justify-center">
        <div class="w-1 bg-yellow-800 h-full relative">
          <div class="absolute top-0 left-1/2 transform -translate-x-1/2 w-4 h-4 bg-yellow-800 rounded-full"></div>
        </div>
      </div>
      <div class="w-1/2">
        <img src={image} alt={name} class="w-32 h-32 object-cover mb-2" />
        <p class="font-semibold">{name}</p>
      </div>
    </div>