<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import * as Card from "$lib/components/ui/card";
  import { CheckIcon, ChevronRightIcon } from "lucide-svelte";
</script>

<div class="bg-white p-8">
  <div class="flex flex-col space-y-8">
    <div
      class="flex items-center md:bg-transparent bg-green-600 text-white p-4"
    >
      <h1 class="text-5xl font-bold text-white md:text-green-600">UPDATES</h1>
    </div>
    <div class="bg-green-600 h-44 w-3/5 absolute right-0 hidden md:block"></div>

    <div class="flex flex-col md:flex-row space-y-8 md:space-y-0 md:space-x-8">
      <div class="flex flex-col space-y-8 md:w-1/3">
        <Card.Root>
          <img
            src="/path-to-podium-image.jpg"
            alt="Campus speaker"
            class="w-full h-48 object-cover"
          />
          <div class="p-4">
            <h3 class="text-xs uppercase text-gray-500">Campus News</h3>
            <h2 class="text-lg font-semibold text-red-600">
              Law School's Diversity Week Features Faculty and Alumni Speakers
            </h2>
          </div>
        </Card.Root>

        <Card.Root>
          <img
            src="/path-to-church-image.jpg"
            alt="Campus building"
            class="w-full h-48 object-cover"
          />
          <div class="p-4">
            <h3 class="text-xs uppercase text-gray-500">Philanthropy</h3>
            <h2 class="text-lg font-semibold text-red-600">
              R.S.H.M./C.S.J. Celebrate 50th Anniversary of Uniport Merger with $1M
              Gifts
            </h2>
          </div>
        </Card.Root>

        <Card.Root>
          <img
            src="/path-to-fountain-image.jpg"
            alt="Campus fountain"
            class="w-full h-48 object-cover"
          />
          <div class="p-4">
            <h3 class="text-xs uppercase text-gray-500">Campus News</h3>
            <h2 class="text-lg font-semibold text-red-600">
              Uniport Awarded 2024 Higher Education Excellence in Diversity Award
            </h2>
          </div>
        </Card.Root>

        <Button
          variant="outline"
          class="w-full hover:bg-green-600 hover:text-white group inline-flex items-center"
          >View All Stories {" "}
            <ChevronRightIcon
              class="ml-1 mt-0.5 h-4 w-4 transition-transform duration-300 group-hover:translate-x-1"
            />
          </Button
        >

      </div>

      <div class="hidden md:flex flex-col space-y-8 md:w-2/3">
        <Card.Root class="relative">
          <img
            src="/path-to-campus-image.jpg"
            alt="Uniport Campus"
            class="w-full h-96 object-cover"
          />
          <div
            class="absolute bottom-0 left-0 right-0 bg-white bg-opacity-90 p-6"
          >
            <h3 class="text-sm uppercase text-gray-500">Press Release</h3>
            <h2 class="text-2xl font-bold">
              Uniport Welcomes New Trustees and Regents
            </h2>
            <p class="mt-2">
              Thirteen new members have joined the Board of Trustees and Board
              of Regents, embracing a new chapter of diverse leadership
              experiences to support the future of Uniport's mission.
            </p>
          </div>
        </Card.Root>

        <div
          class="flex flex-col md:flex-row space-y-8 md:space-y-0 md:space-x-8"
        >
          <Card.Root class="md:w-1/2">
            <img
              src="/path-to-basketball-image.jpg"
              alt="Basketball player"
              class="w-full h-64 object-cover"
            />
            <div class="p-4">
              <h3 class="text-xs uppercase text-gray-500">Athletics</h3>
              <h2 class="text-xl font-semibold">
                2024-25 Men's Basketball Schedule
              </h2>
              <p class="mt-2">
                Uniport Men's Basketball returns to Gersten Pavilion starting Nov. 4
                for a new season.
              </p>
            </div>
          </Card.Root>

          <Card.Root class="md:w-1/2">
            <img
              src="/path-to-professor-image.jpg"
              alt="Professor teaching"
              class="w-full h-64 object-cover"
            />
            <div class="p-4">
              <h3 class="text-xs uppercase text-gray-500">Faculty News</h3>
              <h2 class="text-xl font-semibold text-red-600">
                Playwright Joins CFA Theatre Arts as Assistant Professor
              </h2>
              <p class="mt-2">
                The College of Communication and Fine Arts welcomes David Davila
                as a new assistant professor of playwriting.
              </p>
            </div>
          </Card.Root>
        </div>
      </div>
    </div>
  </div>
</div>
