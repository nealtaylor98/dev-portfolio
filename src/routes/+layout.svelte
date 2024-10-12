<script>
import ContentArea from '$lib/ContentArea.svelte';
import Navbar from '$lib/components/Navbar.svelte';
import '../app.css';
</script>

<Navbar />
<ContentArea>
  <slot></slot>
</ContentArea>

<style></style>
