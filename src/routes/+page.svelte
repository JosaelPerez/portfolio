<script lang="ts">
  import WebLogo from "$lib/components/custom-ui/WebLogo.svelte"
  import ProfileImage from "$lib/components/custom-ui/ProfileImage.svelte"
  import { Button } from "$lib/components/ui/button"
  import * as Dialog from "$lib/components/ui/dialog"
  import * as Carousel from "$lib/components/ui/carousel"
  import * as Card from "$lib/components/ui/card"
  import Autoplay from "embla-carousel-autoplay"
  import { type CarouselAPI } from "$lib/components/ui/carousel/context.js"

  let api: CarouselAPI

  const webLogos = [
    {
      src: "assets/html.svg",
      alt: "HTML Logo",
      caption: "HTML",
    },
    {
      src: "assets/tailwind.svg",
      alt: "Tailwind Logo",
      caption: "Tailwind",
    },
    {
      src: "assets/javascript.svg",
      alt: "Javascript Logo",
      caption: "Javascript",
    },
    {
      src: "assets/svelte.svg",
      alt: "Svelte Logo",
      caption: "Svelte",
    },
    {
      src: "assets/postgresql.svg",
      alt: "PostgreSQL Logo",
      caption: "PostgreSQL",
    },
    {
      src: "assets/prisma.svg",
      alt: "Prisma Logo",
      caption: "Prisma",
    },
    {
      src: "assets/vitejs.svg",
      alt: "ViteJS Logo",
      caption: "ViteJS",
    },
    {
      src: "assets/github.svg",
      alt: "GitHub Logo",
      caption: "GitHub",
    },
    {
      src: "assets/ubuntu.svg",
      alt: "Ubuntu Logo",
      caption: "Linux",
    },
  ]
</script>

<div class="flex h-screen flex-col items-center justify-start">
  <header class="self-stretch">
    <nav class="bg-transparent px-16 py-8">
      <ul class="flex list-none items-center justify-end gap-8 text-white">
        <li class="flex-grow text-2xl">
          <span class="font-bold">Josael</span> Perez
        </li>
        <li>
          <Dialog.Root>
            <Dialog.Trigger
              ><Button class="dark">Get In Touch</Button></Dialog.Trigger>
            <Dialog.Content>
              <Dialog.Header>
                <Dialog.Title>Get In Touch</Dialog.Title>
                <Dialog.Description
                  >Drop me a message on the following platforms.</Dialog.Description>
              </Dialog.Header>
              <ul class="mt-4 flex flex-col items-start gap-2">
                <li>
                  <div>
                    <i
                      class="fa-brands fa-whatsapp fa-lg mr-1"
                      style="color: #222222;"></i
                    ><span class="font-bold">Whatsapp:</span> +52 (686) 2394980
                  </div>
                </li>
                <li>
                  <div>
                    <i
                      class="fa-brands fa-linkedin fa-lg mr-1"
                      style="color: #222222;"></i
                    ><span class="font-bold">LinkedIn:</span>
                    <a
                      href="http://www.linkedin.com/in/josaelprz"
                      class="underline">JosaelPrz</a>
                  </div>
                </li>
                <li>
                  <div>
                    <i
                      class="fa-regular fa-envelope fa-lg mr-1"
                      style="color: #222222;"></i
                    ><span class="font-bold">Gmail:</span> josael.prz@gmail.com
                  </div>
                </li>
              </ul>
            </Dialog.Content>
          </Dialog.Root>
        </li>
      </ul>
    </nav>
  </header>

  <main
    class="flex w-full flex-grow flex-col items-center justify-center overflow-hidden p-0">
    <ProfileImage src="assets/profile.jpg" alt="Josael Perez" />
    <p class="mt-8 text-4xl font-bold text-white">
      Hi! I'm &lcub;Josael&rcub;<span class="text-4xl"> &#129304</span>
    </p>
    <h1 class="text-5xl font-bold text-white">Full Stack Developer</h1>
    <Carousel.Root
      class="dark mt-20 w-full"
      opts={{ loop: true, align: "center", duration: 60 }}
      plugins={[
        Autoplay({
          delay: 2000,
        }),
      ]}>
      <Carousel.Content class="-ml-4">
        {#each webLogos as logo, index}
          <Carousel.Item class="pl-1 md:basis-1/2 lg:basis-1/6">
            <div class="p-1">
              <Card.Root class="border-none bg-transparent">
                <Card.Content
                  class="flex aspect-square items-center justify-center p-6">
                  <WebLogo
                    src={logo.src}
                    alt={logo.alt}
                    caption={logo.caption} />
                </Card.Content>
              </Card.Root>
            </div>
          </Carousel.Item>
        {/each}
      </Carousel.Content>
      <Carousel.Previous />
      <Carousel.Next />
    </Carousel.Root>
  </main>
</div>

<!-- MAIN -->

<!-- FOOTER -->
<footer></footer>
