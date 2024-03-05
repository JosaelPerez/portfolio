<script lang="ts">
  import * as Carousel from "$lib/components/ui/carousel"
  import * as Card from "$lib/components/ui/card"
</script>

<Carousel.Root class="dark h-full" opts={{ align: "center", loop: true }}>
  <Carousel.Content class="absolute inset-0 left-4 -ml-2">
    <Carousel.Item class="pl-0">
      <Card.Root class="h-full rounded-lg border-zinc-700 bg-zinc-950">
        <Card.Content class="flex h-full items-center justify-center p-6">
          <div class="">Hello</div>
        </Card.Content>
      </Card.Root>
    </Carousel.Item>
  </Carousel.Content>
  <Carousel.Previous variant="default" />
  <Carousel.Next variant="default" />
</Carousel.Root>
