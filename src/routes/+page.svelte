<script lang="ts">
  import Navbar from '$lib/navbar.svelte';
  let count: number = 1;
  let name: string = 'Taylor';

  const increment = () => {
    count += 1;
  };
</script>

<div>
  <Navbar />
  <h1>Hello {name}</h1>
  <p>the count is currently {count}</p>
  <button on:click={increment}>Click me</button>
</div>
