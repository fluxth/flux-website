<script lang="ts">
  import type { Snippet } from "svelte";

  import "../app.css";

  type Props = {
    children?: Snippet;
  };

  let { children }: Props = $props();
</script>

<div class="flex min-h-screen items-center justify-center p-3">
  <div class="flex flex-col gap-4 w-full max-w-md">
    {@render children?.()}
  </div>
</div>
