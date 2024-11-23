<script lang="ts">
import Splash from '$lib/components/Splash.svelte';
</script>

<div class="about">
  <Splash
    titleText="Taylor Neal"
    subTitleText="Full Stack Developer"
    buttonHref="/Taylor Neal - Resume.pdf"
    buttonText="Download Resume"
  />
</div>

<style>
.about {
  display: flex;
  flex-direction: column;
  align-items: center;
}

h2 {
  margin-top: 3rem;
}
p {
  margin: 3rem 20rem;
  text-align: center;
}
</style>
