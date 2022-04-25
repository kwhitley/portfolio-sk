<script>
  import { fade, fly } from 'svelte/transition'
  export let refresh = ''
</script>

{#key refresh}
  <div in:fly="{{ x: 300, duration: 500 }}">
    <slot/>
  </div>
{/key}
