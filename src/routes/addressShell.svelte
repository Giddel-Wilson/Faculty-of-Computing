<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import { CheckIcon, ChevronRightIcon } from "lucide-svelte";
</script>

<main class="w-full h-full flex flex-col gap-28 py-32">
  <!-- VC Address Panel -->
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
    <div class="text-center mb-12">
      <p class="text-lg text-gray-600 max-w-3xl mx-auto">
        At LMU, we illuminate new ways of thinking where creativity is boundless
        and justice prevails. Where progress is celebrated. For over a century,
        we've empowered leaders in their ambitious pursuit to secure a brighter
        world for all.
      </p>
    </div>

    <div class="bg-green-600 w-2/5 right-0 h-52 absolute"></div>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12 mb-16">
      <div class="order-2 md:order-1">
        <h2 class="text-4xl font-bold text-green-600 mb-6">
          Vice Chancellor's Address
        </h2>
        <p class="text-gray-700 mb-6 flex flex-col space-y-3">
          <span>Bala blu generated youths umbreleda eba blu eneme super bala down-payment blu mpower umbreleda pdapc roasted recruit agbado blu bulaba different blu mpower corn corn bulaba blu highway bala electricty.</span>
          <span>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error reprehenderit ea perspiciatis a minus, asperiores expedita perferendis rem pariatur eius natus reiciendis obcaecati nulla! Culpa aperiam fuga nihil cumque quasi.
          </span>
        </p>
        <div class="space-y-4 flex flex-col">
          <Button
            variant="outline"
            class="w-fit text-green-600 hover:bg-green-600 hover:text-white group inline-flex items-center"
            >READ MORE {" "}
            <ChevronRightIcon
              class="ml-1 mt-0.5 h-4 w-4 transition-transform duration-300 group-hover:translate-x-1"
            />
            </Button
          >
        </div>
      </div>

      <div class="relative w-full h-full order-1 md:order-2">
        <div class="p-6 z-30">
          <enhanced:img
            src="../assets/VC.jpg"
            alt="Professor Owunari Georgewill"
            class="w-full h-96 object-cover object-top"
          />
        </div>
      </div>
    </div>

    <div class="bg-green-600 w-2/5 left-0 h-52 absolute"></div>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
      <div class="p-6 z-30">
        <enhanced:img
          src="../assets/VC.jpg"
          alt="Professor Owunari Georgewill"
          class="w-full h-96 object-cover object-top"
        />
      </div>
      <div>
        <h2 class="text-4xl font-bold text-green-600 mb-6">Faculty Dean's Address</h2>
        <h3 class="text-2xl font-semibold mb-4">
          Elias Herrera, Social Entrepreneur
        </h3>
        <p class="text-gray-700 mb-6 flex flex-col space-y-3">
          <span>Bala blu generated youths umbreleda eba blu eneme super bala down-payment blu mpower umbreleda pdapc roasted recruit agbado blu bulaba different blu mpower corn corn bulaba blu highway bala electricty.</span>
          <span>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error reprehenderit ea perspiciatis a minus, asperiores expedita perferendis rem pariatur eius natus reiciendis obcaecati nulla! Culpa aperiam fuga nihil cumque quasi.
          </span>
        </p>
        <Button
          variant="outline"
          class="w-fit text-green-600 hover:bg-green-600 hover:text-white group inline-flex items-center"
          >READ MORE {" "}
          <ChevronRightIcon
            class="ml-1 mt-0.5 h-4 w-4 transition-transform duration-300 group-hover:translate-x-1"
          />
          </Button
        >
      </div>
    </div>
  </div>
</main>
