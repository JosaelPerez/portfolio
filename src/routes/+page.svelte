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
  </div>
</main>

<!-- FOOTER -->
<footer></footer>
