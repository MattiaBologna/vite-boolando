<script>
export default {
    data() {
        return {
            itemsList: [
                {
                    defaultImage: '/1.webp',
                    hoverImage: '/1b.webp',
                    discount: 50,
                    sustainability: true,
                    brand: "Levi's",
                    name: 'RELAXED FIT TEE UNISEX',
                    price: '29,99',
                    discountedPrice: '14,99'
                },
                {
                    defaultImage: '/2.webp',
                    hoverImage: '/2b.webp',
                    discount: 30,
                    sustainability: false,
                    brand: 'Guess',
                    name: 'ROSES TEE',
                    price: '29,99',
                    discountedPrice: '20,99'
                },
                {
                    defaultImage: '/3.webp',
                    hoverImage: '/3b.webp',
                    discount: 30,
                    sustainability: false,
                    brand: 'Come zucchero filato',
                    name: 'VOGLIA DI COLORI PASTELLO',
                    price: '184,99',
                    discountedPrice: '129,99'
                },
                {
                    defaultImage: '/4.webp',
                    hoverImage: '/4b.webp',
                    discount: 50,
                    sustainability: true,
                    brand: "Levi's",
                    name: 'TEE UNISEX',
                    price: '29,99',
                    discountedPrice: '14,99'
                },
                {
                    defaultImage: '/5.webp',
                    hoverImage: '/5b.webp',
                    discount: 0,
                    sustainability: true,
                    brand: 'Maya deluxe',
                    name: 'STRIPE BODICE',
                    price: '99,99',
                },
                {
                    defaultImage: '/6.webp',
                    hoverImage: '/6b.webp',
                    discount: 0,
                    sustainability: true,
                    brand: 'Esprit',
                    name: 'MAGLIONE - BLACK',
                    price: '29,99'
                }
            ]
        }
    }
}
</script>

<template>
    <main class="page__content">
        <div class="section">
            <div class="container">
                <div class="row">
                    <div v-for="(item, i) in itemsList" class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img :src="item.defaultImage" alt="">
                                <img :src="item.hoverImage" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                                <div class="badges">
                                    <div v-if="item.discount !== 0" class="discount__badge">-{{ item.discount }}%</div>
                                    <div v-if="item.sustainability" class="sustainability__badge">Sostenibilità</div>
                                </div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">{{ item.brand }}</p>
                                <h3 class="item__name">{{ item.name }}</h3>
                                <p v-if="item.discount !== 0" class="price">{{ item.discountedPrice }}€
                                    <span class="pre-sale-price">{{ item.price }}€</span>
                                </p>
                                <p v-else class="price">{{ item.price }}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped></style>