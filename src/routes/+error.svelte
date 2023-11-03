<script lang="ts">
  import Fa from "svelte-fa";
  import { faHome } from "@fortawesome/free-solid-svg-icons";

  import { page } from "$app/stores";
  import LinkButton from "$lib/components/LinkButton.svelte";
</script>

<svelte:head>
  <title>Error - thitat.net</title>
</svelte:head>

<div class="flex flex-col gap-2 p-4 rounded-lg shadow-lg border">
  <div class="text-center my-4">
    <h1 class="text-3xl font-bold text-neutral-700 mb-1">Something went wrong!</h1>
    <p class="text-neutral-400">{$page.error.message}</p>
  </div>

  <div class="text-center">
    <LinkButton href="/">
      <Fa class="inline mr-1" icon={faHome} />
      Back to homepage
    </LinkButton>
  </div>
</div>
