<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import { Input } from "$lib/components/ui/input";
  import * as Dialog from "$lib/components/ui/dialog";
  import { CheckIcon, ChevronRightIcon } from "lucide-svelte";
</script>

<div class="bg-white px-7 lg:px-12 md:px-0 py-20">
  <div class="flex flex-col md:flex-row w-full max-w-6xl mx-auto shadow-lg">
    <div class="md:w-1/2">
      <img
        src="/placeholder.svg?height=400&width=600"
        alt="Students working on laptops"
        class="w-full h-full object-cover"
      />
    </div>
    <div
      class="md:w-1/2 bg-green-600 text-white p-8 flex flex-col justify-between"
    >
      <div>
        <h2 class="text-4xl font-bold mb-4">Join our Newsletter</h2>
        <p class="text-xl mb-4">
          Lorem ipsum dolor sit amet. Saepe, temporibus.
        </p>
        <div class="mb-6 space-y-3">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt qui
            excepturi beatae totam quis sit pariatur corporis, rerum aliquam
            incidunt. Perspiciatis, odit culpa? Facilis, animi reprehenderit?
          </p>
          <p>
            Incidunt iure quod dicta. Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Enim maxime culpa deleniti veritatis voluptatibus
            officiis esse voluptatem et ad perferendis.
          </p>
        </div>
      </div>
      <div class="flex">
        <Dialog.Root>
          <Dialog.Trigger>
            <Button
              variant="outline"
              class="bg-white text-green-600 hover:text-white hover:bg-green-600 group inline-flex items-center tracking-wider"
            >
              SUBSCRIBE {" "}
              <ChevronRightIcon
                class="ml-1 mt-0.5 h-4 w-4 transition-transform duration-300 group-hover:translate-x-1"
              />
            </Button>
          </Dialog.Trigger>
          <Dialog.Content>
            <Dialog.Header>
              <Dialog.Title>Are you sure absolutely sure?</Dialog.Title>
              <Dialog.Description>
                This action cannot be undone. This will permanently delete your
                account and remove your data from our servers.
              </Dialog.Description>
            </Dialog.Header>
          </Dialog.Content>
        </Dialog.Root>
      </div>
    </div>
  </div>
</div>
