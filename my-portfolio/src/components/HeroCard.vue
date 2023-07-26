<template>
    <section class="hero-card">
        <HeroCardImage />
        <HeroCardIntro />
    </section>
</template>

<script>
import HeroCardImage from '@/components/HeroCardImage.vue';
import HeroCardIntro from '@/components/HeroCardIntro.vue';
export default {
    components: {
        HeroCardImage,
        HeroCardIntro
    }
}
</script>

<style lang="scss" scoped>
.hero-card {
    display: flex;
    justify-content: center;
    flex-direction: row;
    margin-top: 20rem;
    padding: $def_padding;

    @media screen and (max-width: 600px) {
        flex-direction: column;
    }
}
</style>