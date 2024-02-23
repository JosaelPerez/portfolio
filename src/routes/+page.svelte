<script>
  import WebLogo from "$lib/components/custom-ui/WebLogo.svelte"
  import ProfileImage from "$lib/components/custom-ui/ProfileImage.svelte"
</script>

<!-- MAIN -->

<main class="container justify-center">
  <div class="mt-16 flex flex-col items-center">
    <ProfileImage src="assets/profile.jpg" alt="Josael Perez" />
    <p class="mt-8 text-4xl font-bold text-white">
      Hi! I'm &lcub;AJ&rcub;<span class="text-4xl"> &#129304</span>
    </p>
    <h1 class=" mt-2 text-5xl font-bold text-white">Full Stack Developer</h1>
    <div class="mt-24 flex gap-x-24">
      <WebLogo src="assets/html-white.svg" alt="HTML Logo" caption="HTML" />
      <WebLogo
        src="assets/tailwind-white.svg"
        alt="Tailwind Logo"
        caption="Tailwind" />
      <WebLogo
        src="assets/typescript-white.svg"
        alt="TypeScript Logo"
        caption="TypeScript" />
      <WebLogo
        src="assets/svelte-white.svg"
        alt="Svelte Logo"
        caption="Svelte" />
      <WebLogo
        src="assets/postgresql-white.svg"
        alt="PostgreSQL Logo"
        caption="PostgreSQL" />
      <WebLogo src="assets/prisma.svg" alt="Prisma Logo" caption="Prisma" />
      <WebLogo src="assets/github.svg" alt="GitHub Logo" caption="GitHub" />
    </div>
  </div>
</main>

<!-- FOOTER -->
<footer></footer>
