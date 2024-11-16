<script lang="ts">
  import type { Snippet } from "svelte";

  type Props = {
    href: string;
    children?: Snippet;
  };

  let { href, children }: Props = $props();
</script>

<a class="transition text-sky-600 hover:underline hover:text-sky-700" {href}>
  {@render children?.()}
</a>
