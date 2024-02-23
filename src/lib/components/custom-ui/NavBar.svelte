<script>
  import { Button } from "$lib/components/ui/button"
  import * as Sheet from "$lib/components/ui/sheet"
</script>

<header>
  <nav class="bg-transparent px-16 py-8">
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
