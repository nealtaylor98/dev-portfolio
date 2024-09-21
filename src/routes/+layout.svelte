<script>
import PageTitle from '$lib/PageTitle.svelte';
import ContentArea from '$lib/ContentArea.svelte';
import '../app.css';
</script>

<PageTitle />
<ContentArea>
  <slot></slot>
</ContentArea>

<style></style>
