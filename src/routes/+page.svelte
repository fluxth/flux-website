<script lang="ts">
  import LinkButton from "$lib/components/LinkButton.svelte";
</script>

<svelte:head>
  <title>Home - thitat.net</title>
</svelte:head>

<div class="flex min-h-screen items-center justify-center p-3">
  <div class="flex flex-col gap-4 w-full max-w-md">
    <div class="text-center">
      <h1 class="text-3xl font-bold mb-1">thitat.net</h1>
      <p class="text-sm italic text-neutral-400">my website is under construction</p>
    </div>

    <div class="flex flex-col w-full p-2 rounded-lg border shadow-lg text-center">
      <p class="text-xs text-neutral-400 mb-2">reach me on</p>
      <div class="flex flex-col gap-1">
        <LinkButton href="https://github.com/fluxth">GitHub</LinkButton>
        <LinkButton href="https://linkedin.com/in/fluxth">LinkedIn</LinkButton>
        <LinkButton>
          flux<span class="at-prefix">thitat.net</span>
        </LinkButton>
      </div>
    </div>
  </div>
</div>

<style>
  .at-prefix:before {
    content: "@";
  }
</style>
