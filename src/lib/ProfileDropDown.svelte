<script lang="ts">
import { goto } from '$app/navigation';
let isLoggedIn: boolean = false;

function toggleLogin() {
  isLoggedIn = !isLoggedIn; // This is just for demo purposes
}
</script>

<div class="dropdown">
  <div class="dropdown-content">
    {#if isLoggedIn}
      <button class="dropdown-button" on:click={() => goto('/Account')}>Account</button>
      <button class="dropdown-button" on:click={() => goto('/logout')}>Log Out</button>
    {:else}
      <button class="dropdown-button" on:click={() => goto('/login')}>Login</button>
      <button class="dropdown-button" on:click={() => goto('/sign-up')}>Sign Up</button>
    {/if}
  </div>
</div>

<style>
.dropdown {
  position: absolute;
  display: inline-block;
  right: 10vw;
  top: 8vh;
  z-index: 13;
}

.dropdown-content {
  top: 100%;
  right: 10vw;
  background-color: #f9f9f9;
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
  display: flex;
  flex-direction: column;
  z-index: 11;
  border-radius: 14px;
}

.dropdown-button:first-child {
  border-top-right-radius: 14px;
  border-top-left-radius: 14px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}

.dropdown-button:last-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 14px;
  border-bottom-left-radius: 14px;
}

.dropdown-button {
  background-color: none;
  background: none;
  color: black;
  margin: 0;
}

.dropdown-button:hover {
  background-color: var(--page-background);
}
</style>
