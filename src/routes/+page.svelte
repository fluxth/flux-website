<script lang="ts">
  import Fa from "svelte-fa";
  import { faLinkedin, faGithub } from "@fortawesome/free-brands-svg-icons";
  import { faEnvelope } from "@fortawesome/free-solid-svg-icons";

  import LinkButton from "$lib/components/LinkButton.svelte";
  import Link from "$lib/components/Link.svelte";
</script>

<svelte:head>
  <title>Home - thitat.net</title>
</svelte:head>

<div class="text-center">
  <h1 class="text-3xl font-bold text-neutral-700 mb-1">thitat.net</h1>
  <p class="text-sm italic text-neutral-400">this website is under construction</p>
  <p class="text-sm italic text-neutral-400">このホームページはまもなくオープンします</p>
</div>
<div class="flex flex-col w-full p-2 rounded-lg border shadow-lg text-center mb-1">
  <p class="text-xs text-neutral-400 mb-2">reach me on</p>
  <div class="flex flex-col gap-1">
    <LinkButton href="https://github.com/fluxth">
      <Fa class="inline mr-1" icon={faGithub} />
      GitHub
    </LinkButton>
    <LinkButton href="https://linkedin.com/in/fluxth">
      <Fa class="inline mr-1" icon={faLinkedin} />
      LinkedIn
    </LinkButton>
    <LinkButton>
      <Fa class="inline mr-1" icon={faEnvelope} />
      flux<span class="at-prefix">thitat.net</span>
    </LinkButton>
  </div>
</div>
<div class="flex flex-col gap-1 text-center">
  <p class="text-xs text-neutral-400">
    the source code of this website is <Link href="https://github.com/fluxth/flux-website"
      >publicly available</Link
    >
  </p>
  <p class="text-xs text-neutral-400">
    view legacy website at <Link href="https://flux.ci">flux.ci</Link>
  </p>
</div>

<style>
  .at-prefix:before {
    content: "@";
  }
</style>
