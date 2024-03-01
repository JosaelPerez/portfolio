<script lang="ts">
  export let src: string
  export let alt: string
  export let caption: string
  //   export let active: boolean
</script>

<figure
  class="flex min-h-[150px] flex-col items-center justify-between transition-transform duration-300 ease-in-out hover:scale-110">
  <div class="relative flex min-h-[120px] w-32 items-center overflow-hidden">
    <img
      {src}
      {alt}
      class="absolute inset-0 z-20 m-auto w-20 contrast-[10] grayscale-[1]" />
  </div>
  <caption class="block text-2xl font-bold text-white">{caption}</caption>
</figure>
