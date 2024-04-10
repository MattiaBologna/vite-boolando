<script>
export default {
    data() {
        return {
            headerLinks: [
                'Donna',
                'Uomo',
                'Bambini'
            ],
            headerIcons: [
                '/user-solid.svg',
                '/heart-solid.svg',
                '/bag-shopping-solid.svg',
            ]
        }
    }
}
</script>

<template>
    <header class="page__header">
        <nav class="container">
            <div class="row">
                <div class="col-4 text-align-left">
                    <a v-for="(link, i) in headerLinks" class="header-link" href="#">{{ headerLinks[i] }}</a>
                </div>
                <div class="col-4">
                    <a href="#">
                        <img src="/boolean-logo.png" alt="Logo" class="header-logo">
                    </a>
                </div>
                <div class="col-4 text-align-right">
                    <a v-for="(icon, i) in headerIcons" href="#">
                        <img class="header-icons" :src="icon" alt="">
                    </a>
                </div>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped></style>