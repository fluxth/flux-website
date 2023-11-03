<script lang="ts">
  export let href: string;
</script>

<a class="transition text-sky-600 hover:underline hover:text-sky-700" {href}><slot /></a>
