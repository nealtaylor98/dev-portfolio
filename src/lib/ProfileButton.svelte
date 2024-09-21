<script lang="ts">
import { createEventDispatcher } from 'svelte';
import ProfileDropDown from './ProfileDropDown.svelte';

let showProfileDropDown: boolean = false;

function toggleProfileDropdown() {
  showProfileDropDown = !showProfileDropDown;
}
</script>

<div class="component">
  <button class="navbutton profile-button" on:click={toggleProfileDropdown}>
    <i class="light-icon-user title"></i></button
  >

  {#if showProfileDropDown}
    <ProfileDropDown />
  {/if}
</div>

<style>
.profile-button {
  margin-right: 10vw;
}

i {
  font-size: 1.8rem;
}
</style>
