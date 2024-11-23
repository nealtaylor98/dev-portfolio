<script>
import Navlink from './Navlink.svelte';
import Logo from './Logo.svelte';
import Button from './Button.svelte';
</script>

<nav class="navbar">
  <div class="navbar-content">
    <div class="logo">
      <Logo />
    </div>

    <div class="nav-links">
      <Navlink href="/" text="Home" />
      <Navlink href="/portfolio" text="Portfolio" />
      <Navlink href="/blog" text="Blog" />
    </div>

    <div class="hire-button">
      <Button text="Hire Me" />
    </div>
  </div>
</nav>

<style>
.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  background-color: #f8f8f8;
  box-shadow: 0 1px 5px rgba(0, 0, 0, 0.1);
  position: sticky;
  padding: 30px;
  top: 0;
  z-index: 1000;
}

.navbar-content {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.logo {
  position: absolute;
  left: 10vw;
}

.hire-button {
  position: absolute;
  right: 10vw;
}

.nav-links {
  display: flex;
  justify-content: center;
  align-content: center;
  gap: 1rem;
  flex-grow: 1;
}
</style>
