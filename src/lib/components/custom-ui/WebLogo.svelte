<script lang="ts">
  export let src: string
  export let alt: string
  export let caption: string
</script>

<figure class="flex min-h-[150px] flex-col items-center justify-between">
  <div class="flex min-h-[120px] items-center justify-center">
    <img {src} {alt} class="w-[80px]" />
  </div>
  <caption class="block text-2xl font-bold text-white">{caption}</caption>
</figure>
