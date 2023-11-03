<script lang="ts">
  import { page } from "$app/stores";
  import LinkButton from "$lib/components/LinkButton.svelte";
</script>

<div class="flex flex-col gap-2 p-4 rounded-lg shadow-lg border">
  <div class="text-center my-4">
    <h1 class="text-3xl font-bold mb-1">Something went wrong!</h1>
    <p class="text-neutral-400">{$page.error.message}</p>
  </div>

  <LinkButton href="/">Back to homepage</LinkButton>
</div>
