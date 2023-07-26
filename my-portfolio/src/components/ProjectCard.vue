<template>
    <section class="project-card">
        <slot name="projectcard_img"></slot>
        <div></div>
        <section class="content">
            <slot name="projectcard_txt"></slot>
        </section>
    </section>
</template>

<script>
import ProjectCardImage from '@/components/ProjectCardImage.vue';
import ProjectCardText from '@/components/ProjectCardText.vue';
export default {
    components: {
        ProjectCardImage,
        ProjectCardText
    },
    props: {

    }
}
</script>

<style lang="scss" scoped>
.project-card {
    display: flex;
    flex-direction: row;

    @media screen and (max-width: 1440px) {
        flex-direction: column;
    }

    .content {
        padding: 10rem 10rem 10rem 10rem;
        display: flex;
        width: 100%;
        flex-direction: column;
        justify-content: center;
        background: rgb(0, 48, 41);
        background: linear-gradient(90deg, rgba(0, 48, 41, 1) 11%, rgba(0, 118, 102, 1) 100%);

    }

    div {
        width: 160rem;
        margin-left: -80rem;
        background: rgb(9, 31, 30);
        background: linear-gradient(90deg, rgba(9, 31, 30, 0) 0%, rgba(0, 48, 41, 1) 100%);
    }
}
</style>