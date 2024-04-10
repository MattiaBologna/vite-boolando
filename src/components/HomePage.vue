<script>
export default {

}
</script>

<template>
    <header class="page__header">
        <nav class="container">
            <div class="row">
                <div class="col-4 text-align-left">
                    <a class="header-link" href="#">Donna</a>
                    <a class="header-link" href="#">Uomo</a>
                    <a class="header-link" href="#">Bambini</a>
                </div>
                <div class="col-4">
                    <a href="#">
                        <img src="../../public/boolean-logo.png" alt="Logo" class="header-logo">
                    </a>
                </div>
                <div class="col-4 text-align-right">
                    <a href="#">
                        <img class="header-icons" src="../../public//user-solid.svg" alt="">
                    </a>
                    <a href="#">
                        <img class="header-icons" src="../../public//heart-solid.svg" alt="">
                    </a>
                    <a href="#">
                        <img class="header-icons" src="../../public//bag-shopping-solid.svg" alt="">

                    </a>
                </div>
            </div>
        </nav>
    </header>

    <main class="page__content">
        <div class="section">
            <div class="container">
                <div class="row">
                    <div class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img src="../../public//1.webp" alt="">
                                <img src="../../public//1b.webp" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                                <div class="badges">
                                    <div class="discount__badge">-50%</div>
                                    <div class="sustainability__badge">Sostenibilità</div>
                                </div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">Levi's</p>
                                <h3 class="item__name">RELAXED FIT TEE UNISEX</h3>
                                <p class="price">14,99€ <span class="pre-sale-price">29,99€</span></p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img src="../../public//2.webp" alt="">
                                <img src="../../public//2b.webp" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                                <div class="badges">
                                    <div class="discount__badge">-30%</div>
                                </div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">Guess</p>
                                <h3 class="item__name">ROSES TEE</h3>
                                <p class="price">20,99€ <span class="pre-sale-price">29,99€</span></p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img src="../../public//3.webp" alt="">
                                <img src="../../public//3b.webp" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                                <div class="badges">
                                    <div class="discount__badge">-30%</div>
                                </div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">Come Zucchero Filato</p>
                                <h3 class="item__name">VOGLIA DI COLORI PASTELLO</h3>
                                <p class="price">129,99€ <span class="pre-sale-price">184,99€</span></p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img src="../../public//4.webp" alt="">
                                <img src="../../public//4b.webp" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                                <div class="badges">
                                    <div class="discount__badge">-50%</div>
                                    <div class="sustainability__badge">Sostenibilità</div>
                                </div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">Levi's</p>
                                <h3 class="item__name">TEE UNISEX</h3>
                                <p class="price">14,99€ <span class="pre-sale-price">29,99€</span></p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img src="../../public//5.webp" alt="">
                                <img src="../../public//5b.webp" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">Maya Deluxe</p>
                                <h3 class="item__name">STRIPE BODICE</h3>
                                <p class="price">99,99€</p>
                            </div>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="card product">
                            <div class="card__header">
                                <img src="../../public//6.webp" alt="">
                                <img src="../../public//6b.webp" alt="" class="overlay">
                                <div class="fav__heart">&hearts;</div>
                                <div class="badges">
                                    <div class="sustainability__badge">Sostenibilità</div>
                                </div>
                            </div>
                            <div class="card__body">
                                <p class="item__brand">Esprit</p>
                                <h3 class="item__name">MAGLIONE - BLACK</h3>
                                <p class="price">29,99€</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <footer class="page__footer">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <div class="footer-flex">
                        <span class="brand-name col-1">Boolando s.r.l</span>
                        <a class="footer-link" href="#">Informazioni legali</a>
                        <a class="footer-link" href="#">Informazioni sulla privacy</a>
                        <a class="footer-link" href="#">Diritto di recesso</a>
                    </div>
                </div>
                <div class="col-6">
                    <div class="footer-flex text-align-right">
                        <span class="col-1 bold-text">Trovaci anche su</span>
                        <div class="col-1">
                            <a class="social-logos" href="#">
                                <img src="../../public//twitter.svg" alt="">
                            </a>
                            <a class="social-logos" href="#">
                                <img src="../../public//facebook.svg" alt="">
                            </a>
                            <a class="social-logos" href="#">
                                <img src="../../public//instagram.svg" alt="">
                            </a>
                            <a class="social-logos" href="#">
                                <img src="../../public//pinterest.svg" alt="">
                            </a>
                            <a class="social-logos" href="#">
                                <img src="../../public//youtube.svg" alt="">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped></style>