<script lang="ts">
  import type { Snippet } from "svelte";

  type Props = {
    href?: string | undefined;
    children?: Snippet;
  };

  let { href = undefined, children }: Props = $props();

  const commonStyle = "p-2 transition-colors rounded-lg block";
</script>

{#if href}
  <a
    class={`${commonStyle} bg-sky-100/50 text-sky-700 hover:bg-sky-100 active:text-sky-900 active:bg-sky-200`}
    {href}
  >
    {@render children?.()}
  </a>
{:else}
  <span class={`${commonStyle} bg-neutral-100 text-neutral-500 cursor-default`}>
    {@render children?.()}
  </span>
{/if}
