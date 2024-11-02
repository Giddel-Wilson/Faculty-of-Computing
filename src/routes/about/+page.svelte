<script lang="ts">
  import * as Menubar from "$lib/components/ui/menubar";
  import * as Sheet from "$lib/components/ui/sheet/index.js";
  import * as HoverCard from "$lib/components/ui/hover-card";
  import { Label } from "$lib/components/ui/label/index.js";
  import { Button } from "$lib/components/ui/button";
  import { Input } from "$lib/components/ui/input";
  import { Card } from "$lib/components/ui/card";
  import { Search } from "lucide-svelte";

  const categories = [
    "About Overview",
    "Our History",
    "Our Mission",
    "Management",
    "FAQs",
  ];

  const recentArticles = [
    {
      title: "Key Strategies for Previous Study",
      date: "Oct 15, 2023",
    },
    {
      title: "How to Balance Your Research Time",
      date: "Oct 10, 2023",
    },
  ];
</script>

<main class="w-full min-h-screen bg-gray-100">
  <div class="min-h-screen">
    <nav
      class="fixed top-0 w-full h-20 z-50 flex items-center transition-all duration-300 bg-white shadow-md justify-between"
    >
      <div
        class="logos h-full w-max lg:w-1/5 flex items-center gap-1 lg:gap-3 p-5 lg:p-7"
      >
        <span
          ><enhanced:img
            src="/src/assets/nacos.png"
            alt=""
            class="w-14 md:w-16 h-14 md:h-16"
          ></enhanced:img></span
        >
        <span
          ><enhanced:img
            src="/src/assets/uniport.png"
            alt=""
            class="w-12 md:w-14 h-12 md:h-14 hidden lg:block"
          ></enhanced:img></span
        >
        <span>
          <h1 class="text-xl font-bold text-green-600 block lg:hidden">
            NACOS <br /> UNIPORT
          </h1></span
        >
      </div>
      <div
        class="h-full w-3/5 hidden lg:flex justify-center items-center gap-7 font-semibold text-xl transition-all duration-300"
      >
        <Menubar.Root class="bg-transparent py-5">
          <HoverCard.Root>
            <div
              class="flex cursor-default select-none items-center rounded-sm px-3 py-1.5 text-sm font-medium outline-none hover:cursor-pointer hover:text-white hover:bg-green-600"
            >
              <HoverCard.Trigger>
                <a href="../">Home</a>
              </HoverCard.Trigger>
            </div>
          </HoverCard.Root>

          <HoverCard.Root>
            <div
              class="flex cursor-default select-none items-center rounded-sm px-3 py-1.5 text-sm font-medium outline-none hover:cursor-pointer hover:text-white hover:bg-green-600"
            >
              <HoverCard.Trigger>
                <a href="/about">About Us</a>
              </HoverCard.Trigger>
            </div>
          </HoverCard.Root>

          <HoverCard.Root>
            <div
              class="flex cursor-default select-none items-center rounded-sm px-3 py-1.5 text-sm font-medium outline-none hover:cursor-pointer hover:text-white hover:bg-green-600"
            >
              <HoverCard.Trigger>Academics</HoverCard.Trigger>
            </div>
            <HoverCard.Content>
              SvelteKit - Web development, streamlined
            </HoverCard.Content>
          </HoverCard.Root>

          <HoverCard.Root>
            <div
              class="flex cursor-default select-none items-center rounded-sm px-3 py-1.5 text-sm font-medium outline-none hover:cursor-pointer hover:text-white hover:bg-green-600"
            >
              <HoverCard.Trigger>Admission</HoverCard.Trigger>
            </div>
            <HoverCard.Content>
              SvelteKit - Web development, streamlined
            </HoverCard.Content>
          </HoverCard.Root>

          <HoverCard.Root>
            <div
              class="flex cursor-default select-none items-center rounded-sm px-3 py-1.5 text-sm font-medium outline-none hover:cursor-pointer hover:text-white hover:bg-green-600"
            >
              <HoverCard.Trigger>
                <a href="/updates">Updates</a>
              </HoverCard.Trigger>
            </div>
          </HoverCard.Root>

          <HoverCard.Root>
            <div
              class="flex cursor-default select-none items-center rounded-sm px-3 py-1.5 text-sm font-medium outline-none hover:cursor-pointer hover:text-white hover:bg-green-600"
            >
              <HoverCard.Trigger>
                <a href="/contact">Contact Us</a>
              </HoverCard.Trigger>
            </div>
            <HoverCard.Content>
              SvelteKit - Web development, streamlined
            </HoverCard.Content>
          </HoverCard.Root>
        </Menubar.Root>
      </div>
      <div class="h-full w-24 md:w-1/5 flex justify-center items-center">
        <Sheet.Root>
          <Sheet.Trigger asChild let:builder>
            <Button
              builders={[builder]}
              class="bg-transparent w-max h-max block lg:hidden focus:bg-transparent"
            >
              <svg
                class="w-10 h-10"
                viewBox="0 0 24 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                stroke="#16a34a"
                stroke-width="0.36"
                ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
                  id="SVGRepo_tracerCarrier"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></g><g id="SVGRepo_iconCarrier">
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M4 5C3.44772 5 3 5.44772 3 6C3 6.55228 3.44772 7 4 7H20C20.5523 7 21 6.55228 21 6C21 5.44772 20.5523 5 20 5H4ZM7 12C7 11.4477 7.44772 11 8 11H20C20.5523 11 21 11.4477 21 12C21 12.5523 20.5523 13 20 13H8C7.44772 13 7 12.5523 7 12ZM13 18C13 17.4477 13.4477 17 14 17H20C20.5523 17 21 17.4477 21 18C21 18.5523 20.5523 19 20 19H14C13.4477 19 13 18.5523 13 18Z"
                    fill="#16a34a"
                  ></path>
                </g></svg
              >
            </Button>
          </Sheet.Trigger>
          <Sheet.Content side="left" class="flex flex-col justify-between">
            <div>
              <Sheet.Header>
                <Sheet.Title class="mt-3">
                  <div class="flex items-center gap-2">
                    <span
                      ><enhanced:img
                        src="/src/assets/nacos.png"
                        alt=""
                        class="w-14 md:w-16 h-14 md:h-16"
                      ></enhanced:img></span
                    >
                    <span
                      ><enhanced:img
                        src="/src/assets/uniport.png"
                        alt=""
                        class="w-12 md:w-14 h-12 md:h-14"
                      ></enhanced:img></span
                    >
                  </div>
                  <div></div>
                </Sheet.Title>
                <br />
                <hr class="shad" />
              </Sheet.Header>
              <div class="grid gap-5 py-4 mt-5">
                <div>
                  <a
                    href="./"
                    class="flex justify-start items-center gap-4 w-full h-10 p-5 hover:bg-green-600 hover:text-white hover:rounded-md"
                  >
                    <svg
                      viewBox="0 0 24 24"
                      fill="none"
                      class="w-6 h-6"
                      xmlns="http://www.w3.org/2000/svg"
                      ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
                        id="SVGRepo_tracerCarrier"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      ></g><g id="SVGRepo_iconCarrier">
                        <path
                          d="M22 22L2 22"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                          stroke-linecap="round"
                        ></path>
                        <path
                          d="M2 11L6.06296 7.74968M22 11L13.8741 4.49931C12.7784 3.62279 11.2216 3.62279 10.1259 4.49931L9.34398 5.12486"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                          stroke-linecap="round"
                        ></path>
                        <path
                          d="M15.5 5.5V3.5C15.5 3.22386 15.7239 3 16 3H18.5C18.7761 3 19 3.22386 19 3.5V8.5"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                          stroke-linecap="round"
                        ></path>
                        <path
                          d="M4 22V9.5"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                          stroke-linecap="round"
                        ></path>
                        <path
                          d="M20 9.5V13.5M20 22V17.5"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                          stroke-linecap="round"
                        ></path>
                        <path
                          d="M15 22V17C15 15.5858 15 14.8787 14.5607 14.4393C14.1213 14 13.4142 14 12 14C10.5858 14 9.87868 14 9.43934 14.4393M9 22V17"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        ></path>
                        <path
                          d="M14 9.5C14 10.6046 13.1046 11.5 12 11.5C10.8954 11.5 10 10.6046 10 9.5C10 8.39543 10.8954 7.5 12 7.5C13.1046 7.5 14 8.39543 14 9.5Z"
                          stroke="#6b6b6b"
                          stroke-width="1.5"
                        ></path>
                      </g></svg
                    >
                    <Label for="name" class="text-right text-md">Home</Label>
                  </a>
                </div>
                <div>
                  <a
                    href="/about"
                    class="flex justify-start items-center gap-4 w-full h-10 p-5 hover:bg-green-600 hover:text-white hover:rounded-md"
                  >
                    <svg
                      class="w-6 h-6"
                      viewBox="0 0 512 512"
                      version="1.1"
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:xlink="http://www.w3.org/1999/xlink"
                      fill="#000000"
                      ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
                        id="SVGRepo_tracerCarrier"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      ></g><g id="SVGRepo_iconCarrier">
                        <title>about-filled</title>
                        <g
                          id="Page-1"
                          stroke="none"
                          stroke-width="1"
                          fill="none"
                          fill-rule="evenodd"
                        >
                          <g
                            id="drop"
                            fill="#6b6b6b"
                            transform="translate(42.666667, 42.666667)"
                          >
                            <path
                              d="M213.333333,3.55271368e-14 C331.154987,3.55271368e-14 426.666667,95.51168 426.666667,213.333333 C426.666667,331.153707 331.154987,426.666667 213.333333,426.666667 C95.51296,426.666667 3.55271368e-14,331.153707 3.55271368e-14,213.333333 C3.55271368e-14,95.51168 95.51296,3.55271368e-14 213.333333,3.55271368e-14 Z M234.713387,192 L192.04672,192 L192.04672,320 L234.713387,320 L234.713387,192 Z M213.55008,101.333333 C197.99616,101.333333 186.713387,112.5536 186.713387,127.704107 C186.713387,143.46752 197.698773,154.666667 213.55008,154.666667 C228.785067,154.666667 240.04672,143.46752 240.04672,128 C240.04672,112.5536 228.785067,101.333333 213.55008,101.333333 Z"
                              id="Shape"
                            >
                            </path>
                          </g>
                        </g>
                      </g></svg
                    >
                    <Label for="name" class="text-right text-md">About Us</Label
                    >
                  </a>
                </div>
                <div
                  class="flex justify-start items-center gap-4 w-full h-10 p-5 hover:bg-green-600 hover:text-white hover:rounded-md"
                >
                  <svg
                    class="w-6 h-6"
                    viewBox="0 0 1024 1024"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="#000000"
                    ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
                      id="SVGRepo_tracerCarrier"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    ></g><g id="SVGRepo_iconCarrier"
                      ><path
                        fill="#50555b"
                        d="M224 128v704h576V128H224zm-32-64h640a32 32 0 0 1 32 32v768a32 32 0 0 1-32 32H192a32 32 0 0 1-32-32V96a32 32 0 0 1 32-32z"
                      ></path><path
                        fill="#50555b"
                        d="M64 832h896v64H64zm256-640h128v96H320z"
                      ></path><path
                        fill="#50555b"
                        d="M384 832h256v-64a128 128 0 1 0-256 0v64zm128-256a192 192 0 0 1 192 192v128H320V768a192 192 0 0 1 192-192zM320 384h128v96H320zm256-192h128v96H576zm0 192h128v96H576z"
                      ></path></g
                    ></svg
                  >
                  <Label for="name" class="text-right text-md">Academics</Label>
                </div>
                <div
                  class="flex justify-start items-center gap-4 w-full h-10 p-5 hover:bg-green-600 hover:text-white hover:rounded-md"
                >
                  <svg
                    class="w-6 h-6"
                    viewBox="0 0 24 24"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                    ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
                      id="SVGRepo_tracerCarrier"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    ></g><g id="SVGRepo_iconCarrier">
                      <path
                        d="M21 10L12 5L3 10L6 11.6667M21 10L18 11.6667M21 10V10C21.6129 10.3064 22 10.9328 22 11.618V16.9998M6 11.6667L12 15L18 11.6667M6 11.6667V17.6667L12 21L18 17.6667L18 11.6667"
                        stroke="#50555b"
                        stroke-width="2"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      ></path>
                    </g></svg
                  >
                  <Label for="name" class="text-right text-md">Addmission</Label
                  >
                </div>
                <div>
                  <a
                    href="/updates"
                    class="flex justify-start items-center gap-4 w-full h-10 p-5 hover:bg-green-600 hover:text-white hover:rounded-md"
                  >
                    <svg
                      class="w-6 h-6"
                      fill="#6b6b6b"
                      viewBox="0 0 24 24"
                      xmlns="http://www.w3.org/2000/svg"
                      stroke="#6b6b6b"
                      ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
                        id="SVGRepo_tracerCarrier"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      ></g><g id="SVGRepo_iconCarrier">
                        <path
                          d="M16 2H8C7.46957 2 6.96086 2.21071 6.58579 2.58579C6.21071 2.96086 6 3.46957 6 4H15V9H20V20H6C6 20.5304 6.21071 21.0391 6.58579 21.4142C6.96086 21.7893 7.46957 22 8 22H20C20.5304 22 21.0391 21.7893 21.4142 21.4142C21.7893 21.0391 22 20.5304 22 20V8L16 2Z"
                        ></path>
                        <path
                          d="M11.3245 14.4883L12.6906 15.822V16.4942H2V15.822L3.3553 14.4883V11.1597C3.28833 10.2186 3.55162 9.28363 4.09982 8.51576C4.64802 7.74789 5.44681 7.1952 6.35864 6.95288V6.4975C6.35864 6.23295 6.46373 5.97923 6.6508 5.79216C6.83787 5.60509 7.09159 5.5 7.35614 5.5C7.62069 5.5 7.87441 5.60509 8.06148 5.79216C8.24855 5.97923 8.35364 6.23295 8.35364 6.4975V6.95288C9.25835 7.20335 10.0485 7.75916 10.59 8.52597C11.1315 9.29278 11.391 10.2233 11.3245 11.1597V14.4883Z"
                        ></path>
                        <path
                          d="M8.26662 18.1094C8.01652 18.3595 7.67731 18.5 7.32361 18.5C6.96992 18.5 6.63071 18.3595 6.3806 18.1094C6.1305 17.8593 5.99 17.5201 5.99 17.1664H8.65722C8.65722 17.5201 8.51672 17.8593 8.26662 18.1094Z"
                        ></path>
                      </g></svg
                    >
                    <Label for="name" class="text-right text-md">Updates</Label>
                  </a>
                </div>
              </div>
            </div>
            <Sheet.Footer>
              <Sheet.Close asChild let:builder>
                <Button builders={[builder]} type="submit" class="bg-green-600">
                  <a href="/contact" class="w-full h-full"> Contact Us </a>
                </Button>
              </Sheet.Close>
            </Sheet.Footer>
          </Sheet.Content>
        </Sheet.Root>
      </div>
    </nav>

    <div class="mt-20">
      <!-- Header Section -->
      <div
        class="bg-green-600 p-8 w-auto absolute z-20 mt-56 right-0 md:right-auto md:left-5 lg:left-32
                                                                                                                                                                "
      >
        <div class="text-white/80 uppercase text-sm tracking-wide">About</div>
        <h1 class="text-white font-bold text-2xl md:text-3xl mt-2">
          About the faculty
        </h1>
      </div>

      <!-- Banner Image -->
      <div class="w-full h-[300px] relative">
        <enhanced:img
          src="/src/assets/background2.jpg"
          alt="Students enjoying campus life"
          class="w-full h-full object-cover"
        />
      </div>
    </div>
    <main class="container mx-auto px-4 mb-10 pt-20">
      <h1 class="text-4xl font-bold mb-4">About Overview</h1>
      <div class="min-h-screen bg-white">
        <!-- Hero Section -->
        <div class="relative h-[400px] w-full bg-cover bg-center bg-no-repeat bg-gradient-to-r from-green-600 to-black">
          <enhanced:img
            src="/src/assets/wallpaperflare.com_wallpaper.jpg"
            alt="Facukty Building"
            class="w-full h-full object-cover bg-gray-900 opacity-80"
          />
          <div
            class="absolute inset-0 bg-navy/60 flex items-center justify-center"
          >
            <div class="text-center text-white shadow-lg">
              <div class="text-sm uppercase tracking-wider mb-2 font-semibold">
                ABOUT
              </div>
              <h1 class="text-4xl font-extrabold max-w-2xl">
                Everything you need to know about The Faculty of Computing.
              </h1>
            </div>
          </div>
        </div>

        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 py-8">
          <div class="flex gap-8 flex-col lg:flex-row">
            <!-- Article Content -->
            <div class="flex-grow">
              <!-- Article Text -->
              <div class="prose max-w-none">
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Id magnam molestiae eum incidunt eius nesciunt exercitationem, iure laudantium possimus culpa necessitatibus earum, in qui et laboriosam debitis, corrupti ipsam dolorum. Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde repellat tempora eum voluptatibus dignissimos cum aut culpa nihil quia cupiditate.
                </p>


                <div class="flex flex-col md:flex-row items-center gap-8 p-6 max-w-7xl mx-auto my-10">
                  <div class="flex-shrink-0 w-full lg:w-[400px] h-full lg:h-[400px]">
                    <enhanced:img
                      src="/src/assets/file2.png"
                      alt="NACOS Logo"
                      class="w-full h-full object-contain"
                    />
                  </div>
                  
                  <div class="flex flex-col gap-6 flex-1">
                    <p>
                      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cum accusamus deleniti fugit dolorem aut beatae, dignissimos eos impedit ex. Laborum esse assumenda error necessitatibus quas officiis minima maxime consectetur nostrum! Lorem ipsum dolor, sit amet consectetur adipisicing elit. Optio quia pariatur, non obcaecati ex atque nostrum minus. Laboriosam vitae blanditiis et, voluptatem necessitatibus beatae voluptas voluptatibus, architecto magni facilis eveniet? Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quisquam expedita voluptatum id deserunt eveniet possimus.
                    </p>
                    
                    <div>
                      <Button 
                        variant="default" 
                        class="bg-green-600 hover:bg-green-700 text-white font-medium px-8 py-2 rounded-full"
                      >
                        READ MORE
                      </Button>
                    </div>
                  </div>
                </div>

                <!-- <enhanced:img
                  src="/placeholder.svg?height=300&width=800"
                  alt="STEM Lab Equipment"
                  class="my-6 w-full rounded-lg"
                />

                <p>
                  The new STEM lab features advanced equipment, including 3D
                  printers, robotics kits, and state-of-the-art microscopes.
                  These tools will enable students to engage in hands-on
                  learning and conduct complex experiments.
                </p> -->
              </div>
            </div>

            <!-- Sidebar -->
            <div class="w-80 flex-shrink-0">
              <!-- Search -->
              <Card class="p-4 mb-6">
                <h2 class="font-semibold mb-4">Search Bar</h2>
                <div class="flex gap-2">
                  <Input placeholder="Enter your search..." />
                  <Button variant="outline" size="icon">
                    <Search class="h-4 w-4" />
                  </Button>
                </div>
              </Card>

              <!-- Categories -->
              <Card class="p-4 mb-6">
                <h2 class="font-semibold mb-4">Categories</h2>
                <ul class="space-y-2">
                  {#each categories as category}
                    <li>
                      <a
                        href="#{category.toLowerCase().replace(' ', '-')}"
                        class="text-sm text-muted-foreground transition-colors hover:text-green-600"
                      >
                        {category}
                      </a>
                    </li>
                  {/each}
                </ul>
              </Card>

              <!-- Recent Articles -->
              <Card class="p-4">
                <h2 class="font-semibold mb-4">Recent Articles</h2>
                <ul class="space-y-4">
                  {#each recentArticles as article}
                    <li>
                      <a
                        href="#{article.title.toLowerCase().replace(' ', '-')}"
                        class="block hover:bg-muted p-2 rounded-lg transition-colors"
                      >
                        <div class="font-medium text-sm">{article.title}</div>
                        <div class="text-xs text-muted-foreground">
                          {article.date}
                        </div>
                      </a>
                    </li>
                  {/each}
                </ul>
              </Card>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>

  <footer class="bg-green-600 text-white p-4 mt-8 text-center">
    <p class="mb-1 md:mb-0 text-center">
      Copyright © NACOS UNIPORT 2024/2025 . All Right Reserved.
    </p>
  </footer>
</main>
