<script>
export default {
    props: ['product']
}
</script>

<template>
    <div class="card product">
        <div class="card__header">
            <img :src="'/' + product.frontImage" alt="">
            <img :src="'/' + product.backImage" alt="" class="overlay">
            <div class="fav__heart">&hearts;</div>
            <div class="badges">
                <div v-for="(badge, i) in product.badges" :key="i" :class="`badge__${badge.type}`">
                    {{ badge.value }}</div>
            </div>
        </div>
        <div class="card__body">
            <p class="item__brand">{{ product.brand }}</p>
            <h3 class="item__name">{{ product.name }}</h3>
            <!-- <p v-if="item.discount !== 0" class="price">{{ item.discountedPrice }}€ -->
            <!-- <span class="pre-sale-price">{{ item.price }}€</span> -->
            <!-- </p> -->
            <!-- <p v-else class="price">{{ item.price }}</p> -->
        </div>
    </div>
</template>

<style></style>