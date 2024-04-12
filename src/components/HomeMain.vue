<script>
import ItemCard from './ItemCard.vue';
import { store } from '../store.js';

export default {
    components: {
        ItemCard,
    },
    data() {
        return {
            products: store.products,
            components: {
                ItemCard
            },
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
                    <!-- <ItemCard /> -->
                    <div v-for="product in products" class="col-4" :key="product.id">
                        <ItemCard :product="product" />
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped></style>