<template>
    <article class="intro-text">
        <p class="intro-hello">
            Hi, mein Name ist Niklas Peper.
        </p>
        <h1>
            Ich bin ein Frontend-Developer<br>& UI/UX-Designer.
        </h1>
        <p class="content">
            Ich habe kürzlich mein Studium in Medieninformatik abgeschlossen (M.Sc.) und bin auf der Suche nach einem
            spannenden Job.
        </p>
    </article>
</template>

<script>

export default {
}
</script>

<style lang="scss" scoped>
.intro-text {
    color: $color_heading;
    max-width: 40rem;

    p {
        font-size: $size_paragraph;
        padding: 0;
        margin: 0;

        &.intro-hello {
            margin: 2rem 0 1rem 0;
        }

        &.content {
            margin: 0 0 2rem 0;
            line-height: $lineheight_paragraph;
            color: grey;
        }
    }

    h1 {
        font-size: 2.5rem;
        padding: 0;
        margin: 0 0 1rem 0;
    }
}
</style>