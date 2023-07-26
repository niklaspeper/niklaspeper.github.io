<script>

import HeroCard from '@/components/HeroCard.vue';
export default {
  components: {
    HeroCard
  }

}

</script>

<template>
  <main>
    <HeroCard />
  </main>
</template>

<style lang="scss">
@font-face {
  font-family: $nunito;
  src: url('@/assets/fonts/Nunito-Regular.ttf');
  font-weight: 500;
}

@font-face {
  font-family: $nunito_sans_reg;
  src: url('@/assets/fonts/NunitoSans_10pt-Regular.ttf');
  font-weight: 500;
}

body,
html {
  font-family: $nunito_sans_reg;
  background-color: $color_bg;
  font-size: 10px;
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

* {
  box-sizing: border-box;
}
</style>
