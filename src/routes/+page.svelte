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
  <h2>About Me</h2>
  <p>
    G’day! I’m Taylor, a software engineer with a knack for crafting innovative solutions. While
    I’ve honed my skills through professional experience for over a year, my journey in software
    development spans nearly five. My expertise lies in full-stack application development, where I
    thrive on bringing ideas to life through code. When I’m not at work, you’ll find me developing
    games in my spare time and having a crack at new languages and technologies to broaden my
    skillset. I’m always up for taking on new challenges and keen to continue sharpening my mind and
    skills!
  </p>
  <p></p>
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
