<script lang="ts">
export let text: string = '';
export let buttonHref: string | null | undefined = undefined;
export let buttonClick: () => void = () => {};
</script>

{#if buttonHref}
  <a href={buttonHref} download>
    <button class="download-button">{text}</button>
  </a>
{:else}
  <button class="download-button" on:click={buttonClick}>{text}</button>
{/if}

<style>
</style>
