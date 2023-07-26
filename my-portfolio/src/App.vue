<script>

import HeroCard from '@/components/HeroCard.vue';
import Footer from '@/components/Footer.vue';
import ProjectCard from '@/components/ProjectCard.vue';
import ProjectCardImage from '@/components/ProjectCardImage.vue';
import ProjectCardText from '@/components/ProjectCardText.vue';

export default {
  components: {
    HeroCard,
    Footer,
    ProjectCard,
    ProjectCardImage,
    ProjectCardText
  }

}

</script>

<template>
  <main>
    <HeroCard />
    <p class="my-projects-heading">Bisherige Projekte</p>

    <!-- Projekt #1 -->
    <ProjectCard>
      <template #projectcard_img>
        <ProjectCardImage>
          <img class="projectcard-img" src="@/assets/images/vr-concept.gif" alt="VR Zeitsteuerung Interface">
        </ProjectCardImage>
      </template>
      <template #projectcard_txt>
        <ProjectCardText>
          <h1 class="projectcard-heading">#1 Masterarbeit</h1>
          <p class="projectcard-text">
            "Kontextsensitive Steuerung der Zeit in Virtual Reality am
            Beispiel von Bauablaufsimulationen".
          </p>
          <img class="vr-icon" src="@/assets/icons/VR_Icon.svg" alt="VR-Icon">
        </ProjectCardText>
      </template>
    </ProjectCard>
  </main>
  <Footer />
</template>

<style lang="scss">
@font-face {
  font-family: $nunito;
  src: url('@/assets/fonts/Nunito-Regular.ttf');
  font-weight: 500;
}

@font-face {
  font-family: $nunito_sans;
  src: url('@/assets/fonts/NunitoSans_10pt-Regular.ttf');
  font-weight: 500;
}


body,
html {
  font-family: $nunito_sans;
  background-color: $color_bg;
  font-size: 10px;
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  // align-items: center;
  flex-direction: column;
  height: auto;
}

* {
  box-sizing: border-box;
}

.my-projects-heading {
  font-family: $nunito_sans;
  font-size: $size_heading;
  font-weight: bold;
  display: flex;
  justify-content: center;
  margin: 10rem 0 10rem 0;
  padding: $def_padding;
}

.projectcard-img {
  width: 100rem;
  margin-left: -10rem;

  @media screen and (max-width: 1440px) {
    width: 100%;
    margin: 0;
  }

}

.projectcard-heading {
  font-size: $size_heading;
  margin: 0 0 10rem 0;
}

.projectcard-text {
  font-size: $size_projecttext;
  line-height: $lineheight_projecttext;
  font-style: italic;
}

.vr-icon {
  width: 10rem;
}
</style>
