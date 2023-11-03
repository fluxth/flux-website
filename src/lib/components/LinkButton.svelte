<script lang="ts">
  export let href: string | undefined = undefined;

  let commonStyle = "p-2 transition-colors rounded-lg block";
</script>

{#if href}
  <a
    class={`${commonStyle} bg-sky-100/50 text-sky-700 hover:bg-sky-100 active:text-sky-900 active:bg-sky-200`}
    {href}><slot /></a
  >
{:else}
  <span class={`${commonStyle} bg-neutral-100 text-neutral-500 cursor-default`}><slot /></span>
{/if}
