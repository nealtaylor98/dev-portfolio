<script lang="ts">
  let count: number = 0;
  let name: string = 'Taylor';

  const increment = () => {
    count += 1;
  };
</script>

<div>
  <h1>Hello {name}</h1>
  <p>the count is currently {count}</p>
  <button on:click={increment}>Click
    me</button>

</div>
