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
      <Navlink href="/services" text="Services" />
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
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: #f8f8f8;
  box-shadow: 0 1px 5px rgba(0, 0, 0, 0.1);
}

.navbar-content {
  margin-left: 2vw;
  margin-right: 2vw;
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-around;
}

.nav-links {
  display: flex;
  align-content: center;
  gap: 1rem;
  margin-left: 1vw;
  margin-right: 8vw;
}
</style>
