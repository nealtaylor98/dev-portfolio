<script>
export let href = '';
export let text = '';
</script>

<a {href} class="nav-link">
  {text}
</a>

<style>
.nav-link {
  text-decoration: none;
  color: black;
  font-weight: bold;
  font-weight: 500;
}

.nav-link:hover {
  color: #6200ea;
}
</style>
