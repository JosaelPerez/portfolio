<script>
  import WebLogo from "$lib/components/custom-ui/WebLogo.svelte"
  import ProfileImage from "$lib/components/custom-ui/ProfileImage.svelte"
  import { Button } from "$lib/components/ui/button"
  import * as Sheet from "$lib/components/ui/sheet"
</script>

<div class="flex h-screen flex-col items-center justify-start">
  <header class="self-stretch">
    <nav class="border bg-transparent px-16 py-8">
      <ul class="flex list-none items-center justify-end gap-8 text-white">
        <li class="flex-grow text-2xl">
          <span class="font-bold">Josael</span> Perez
        </li>
        <li>
          <Sheet.Root>
            <Sheet.Trigger asChild let:builder>
              <Button builders={[builder]} class="dark">Get in touch</Button>
            </Sheet.Trigger>
            <Sheet.Content side="right" class="dark">
              <Sheet.Header>
                <Sheet.Title>Get In Touch</Sheet.Title>
                <Sheet.Description
                  >Drop me a message on the following platforms.</Sheet.Description>
              </Sheet.Header>
              <div class="">
                <ul class="mt-4 flex flex-col items-start gap-2">
                  <li>
                    <Button
                      ><i
                        class="fa-brands fa-whatsapp fa-lg mr-1"
                        style="color: #222222;"></i
                      >Whatsapp</Button>
                  </li>
                  <li>
                    <Button
                      ><i
                        class="fa-brands fa-linkedin fa-lg mr-1"
                        style="color: #222222;"></i
                      >LinkedIn</Button>
                  </li>
                  <li>
                    <Button
                      ><i
                        class="fa-regular fa-envelope fa-lg mr-1"
                        style="color: #222222;"></i
                      >Gmail</Button>
                  </li>
                </ul>
              </div>
            </Sheet.Content>
          </Sheet.Root>
        </li>
      </ul>
    </nav>
  </header>

  <main
    class="container flex flex-grow flex-col items-center justify-center border p-0">
    <ProfileImage src="assets/profile.jpg" alt="Josael Perez" />
    <p class="mt-8 border text-4xl font-bold text-white">
      Hi! I'm &lcub;Josael&rcub;<span class="text-4xl"> &#129304</span>
    </p>
    <h1 class="border text-5xl font-bold text-white">Full Stack Developer</h1>
    <div class="mt-24 flex items-center justify-around self-stretch border">
      <WebLogo
        mainSource="assets/html-gray.svg"
        secondarySource="assets/html.svg"
        alt="HTML Logo"
        caption="HTML" />
      <WebLogo
        mainSource="assets/tailwind-gray.svg"
        secondarySource="assets/tailwind.svg"
        alt="Tailwind Logo"
        caption="Tailwind" />
      <WebLogo
        mainSource="assets/javascript-gray.svg"
        secondarySource="assets/javascript.svg"
        alt="Javascript Logo"
        caption="Javascript" />
      <WebLogo
        mainSource="assets/svelte-gray.svg"
        secondarySource="assets/svelte.svg"
        alt="Svelte Logo"
        caption="Svelte" />
      <WebLogo
        mainSource="assets/postgresql-gray.svg"
        secondarySource="assets/postgresql.svg"
        alt="PostgreSQL Logo"
        caption="PostgreSQL" />
      <WebLogo
        mainSource="assets/prisma.svg"
        alt="Prisma Logo"
        caption="Prisma" />
      <WebLogo
        mainSource="assets/github.svg"
        alt="GitHub Logo"
        caption="GitHub" />
    </div>
  </main>
</div>

<!-- MAIN -->

<!-- FOOTER -->
<footer></footer>
