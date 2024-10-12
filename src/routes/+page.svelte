<script lang="ts">
import Splash from '$lib/components/Splash.svelte';

function downloadResume() {}
</script>

<div class="about">
  <Splash
    titleText="Taylor Neal"
    subTitleText="Full Stack Developer"
    buttonClick={downloadResume}
    buttonText="Download Resume"
  />
  <h2>About Me</h2>
  <p>
    Hello! I'm Taylor, a passionate software engineer who's been developing software for over 3
    years. My expertise lies in full stack application development, where I enjoy bringing ideas to
    life through code. I also enjoy developing games in my free time as well as experimenting with
    other languages/technologies.
  </p>
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
