<template>
    <article class="project-text">
        <slot></slot>
    </article>
</template>

<script>
export default {
    components: {
    }
}
</script>

<style lang="scss" scoped>
.project-text {
    color: $color_bg;
    max-width: 40rem;

}
</style>