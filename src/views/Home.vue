<template>
    <div class="homePage">
        <div class="homeSlider">
            <splide :options="options" class="slider">
                <splide-slide class="slider_item">
                    <img src="../assets/img/slider.png">
                    <div class="sliderText">Ребрендинг <br> диджитал агенства</div> 
                    <div class="sliderOrder">Клиент: Rocket</div>
                    
                </splide-slide>
                <splide-slide class="slider_item">
                    <img src="../assets/img/slider.png">
                    <div class="sliderText">Ребрендинг <br> диджитал агенства</div>
                    <div class="sliderOrder">Клиент: Rocket</div>
                    
                </splide-slide>
                <splide-slide class="slider_item">
                    <img src="../assets/img/slider.png">
                    <div class="sliderText">Ребрендинг <br> диджитал агенства</div>
                    <div class="sliderOrder">Клиент: Rocket</div>
                    
                </splide-slide>
                <splide-slide class="slider_item">
                    <img src="../assets/img/slider.png">
                    <div class="sliderText">Ребрендинг <br> диджитал агенства</div>
                    <div class="sliderOrder">Клиент: Rocket</div>            
                </splide-slide>
        
            </splide>
            
            <router-link to="projects" class="sliderBtn">Все проекты</router-link>
        </div>
        <div class="whiteFooter">
            <div class="whiteFooter_left">
                <router-link to="/" class="whiteFooter_left_logo">
                    <img src="../assets/img/logoBig.png" alt="">
                </router-link>
                <div class="whiteFooter_left_text">© 2020 Taboo Branding Bureau</div>
            </div>
            <div class="whiteFooter_right">
                <div class="whiteFooter_right_top">
                    Мирабадский район, ул. Афросиеб, 13, 3-й этаж. Ориентир: UzbeGYM, метро Ойбек.
                </div>
                <div class="whiteFooter_right_bottom">
                    Телефон: +998 90 9800178 Telegram: mssg.me/taboodsgn
                </div>
            </div>
        </div>

    </div>
</template>




<script>

import { Splide, SplideSlide } from '@splidejs/vue-splide'


export default {
    components: {
        Splide,
        SplideSlide,
        
    },
    data() {
        return {
            options: {
                drag: true,
                type: 'loop',
                rewind: true,
				perPage: 1,
                arrows: true,
                autoplay: true,
                interval: 3000,
                keyboard: true,
                
			},
        }
    },
}
</script>

<style lang="scss">

@import url(../assets/scss/style.scss);


</style>