<script lang="ts">
// Props
export let icon: string | any;
export let name: string;
</script>

<div class="tech-item">
  {#if typeof icon === 'string'}
    <span class="icon">{icon}</span>
  {:else}
    <svelte:component this={icon} />
  {/if}
  <span class="name">{name}</span>
</div>

<style>
.tech-item {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  padding: 0.75rem 1rem;
  background-color: var(--primary);
  border-radius: 0.5rem;
  box-shadow: var(--shadow);
  transition: all 0.2s ease-in-out;
}

.tech-item:hover {
  background-color: var(--secondary);
  translate: 0px -2px;
}

.icon {
  color: var(--accent);
  font-size: 1.25rem;
}

.name {
  color: var(--highlight);
  font-size: 1rem;
  font-weight: 500;
}
</style>

