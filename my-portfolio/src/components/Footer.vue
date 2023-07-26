<template>
    <footer>
        <p>{{ currentYear }} Copyright by Niklas Peper. Created with Vue.</p>
    </footer>
</template>

<script>

export default {
    data() {
        return {
            currentYear: new Date().getFullYear()
        }
    },
}
</script>

<style lang="scss" scoped>
footer {
    display: flex;
    justify-content: center;
    margin: 5rem 0 0 0;

    p {
        font-size: 1.2rem;
        color: grey;
    }

}
</style>