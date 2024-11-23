<script lang="ts">
// Props for customization
export let columns: number = 4;
export let gap: string = '1rem';
export let minItemWidth: number = 200;
export let width: string = '100';
</script>

<div
  class="grid-container"
  style="--columns: {columns}; 
         --gap: {gap}; 
         --min-item-width: {minItemWidth}px;
         --grid-width: {width};"
>
  <slot />
</div>

<style>
.grid-container {
  display: grid;
  /* Use repeat with auto-fill for responsive behavior */
  grid-template-columns: repeat(var(--columns), 1fr);
  gap: var(--gap);
  width: var(--grid-width);
  padding: 1rem;
  background: none;
  border-radius: 0.5rem;
}

/* For smaller screens, switch to auto-fit for responsiveness */
@media (max-width: 768px) {
  .grid-container {
    grid-template-columns: repeat(auto-fit, minmax(var(--min-item-width), 1fr));
    padding: 0.5rem;
  }
}
</style>

