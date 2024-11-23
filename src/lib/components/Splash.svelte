<script lang="ts">
import Button from './Button.svelte';
import Grid from './Grid.svelte';
import TechItem from './TechItem.svelte';

export let titleText: string;
export let subTitleText: string;
export let buttonText: string;
export let buttonHref: string;
export let buttonClick: () => void = () => {};
export let imageUrl: string = '/header-image.jpg';
</script>

<div class="splash">
  <div class="splash-bg" style="background: url({imageUrl}) no-repeat center center"></div>

  <div class="splash-content-area">
    <div class="splash-content">
      <h1>{titleText}</h1>
      <h2>{subTitleText}</h2>
      <Grid columns={2} width="50%">
        <TechItem icon="A" name="React" />
        <TechItem icon="A" name=".NET" />
        <TechItem icon="A" name="Node" />
        <TechItem icon="A" name="Svelte" />
      </Grid>
      <Button text={buttonText} {buttonHref} />
    </div>
  </div>
</div>

<style>
.splash {
  position: relative;
  width: 100%;
  height: 90vh;
  overflow: hidden;
  align-items: center;
  justify-content: center;
  align-content: center;
}

.splash-bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-size: cover;
  filter: blur(10px);
  z-index: 1;
}

h2 {
  margin: 2rem 0;
}

h1 {
  color: white;
}

.splash-content-area {
  background: rgba(0, 0, 0, 0.4);
  position: relative;
  z-index: 2;
  width: 100%;
  height: 100%;
  display: flex;
}

.splash-content {
  padding-right: 5000px;
  color: white;
  padding: 2rem;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
