<script lang="ts">
  export let mainSource: string
  export let secondarySource: string | undefined = undefined
  export let alt: string
  export let caption: string
</script>

<figure
  class="flex min-h-[150px] flex-col items-center justify-between transition-transform duration-200 ease-out hover:scale-110">
  <div class="relative flex min-h-[120px] w-32 items-center overflow-hidden">
    <img
      src={mainSource}
      {alt}
      class="absolute inset-0 z-20 m-auto w-20 hover:z-0" />
    {#if secondarySource}
      <img
        src={secondarySource}
        {alt}
        class="absolute inset-0 z-10 m-auto w-20 hover:z-30" />
    {/if}
  </div>
  <caption class="block text-2xl font-bold text-white">{caption}</caption>
</figure>
