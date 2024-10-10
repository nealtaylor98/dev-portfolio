<script lang="ts">
import { goto } from '$app/navigation';

function returnHome() {
  goto('/');
}
</script>

<div>
  <div class="component">
    <button class="navbutton home-button" on:click={returnHome}>
      <i class="light-icon-home title"></i></button
    >
    <h1 class="title">Rustbound Adventures</h1>
  </div>
</div>

<style>
.component {
  background-image: radial-gradient(var(--background), var(--primary));
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  margin: 0;
  padding: 5;
  height: 10vh;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-align: center;
  z-index: 10;
}

.title {
  color: #f4f4f4;
}

i {
  font-size: 1.8rem;
  margin: 0;
  padding: 0;
}

.home-button {
  margin-left: 10%;
}
</style>
