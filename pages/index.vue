<template>
    <section id="accueil" class="container">
        <h1>Grapucine</h1>
        <p>paris</p>
        <a class="btn" href="/#contact">Visitez</a>
        <span class="modelName">Model : Abir Hamdi</span>
    </section>

    <section id="notre-histoire">
        <div class="imgContainer left">
            <img src="../public/img/stepan-kulyk.png" alt="Stepan Kulyk">
            <span class="modelName">Photo : Stepan Kulyk</span>
        </div>
        <div class="content">
            <h2 class="hiddenDesktop"><span>Notre</span> Histoire</h2>
            <p>
                <strong>Paris</strong> est la ville de la mode par excellence et une destination incontournable pour tous les amoureux de la mode. Si vous cherchez à percer dans <strong>l'industrie de la mode</strong> en tant que mannequin, il n'y a pas de meilleur endroit pour commencer que dans une <strong>agence de mannequin</strong> à Paris.
            </p>
            <p>
                Notre agence de mannequin située au cœur de <strong>Paris est fiere de representer</strong> les meilleurs modèles de la ville. Nous avons une équipe de professionnels expérimentés qui sont passionnés par leur travail et qui ont une <strong>connaissance approfondie</strong> de l'industrie de la mode.
            </p>
        </div>
        <div class="imgContainer right">
            <img src="../public/img/omid-armin.png" alt="Omid Armin">
            <span class="modelName">Photo: Omid Armin </span>
        </div>
    </section>
    
    <section id="galerie">
        <div class="slider">
            <swiper
            :slides-per-view="1"
            :space-between="0"
            @swiper="onSwiper"
            @slideChange="onSlideChange"
            
        >
            <swiper-slide>
                <div class="imgSlide slide_1"></div>
            </swiper-slide>
            <swiper-slide>
                <div class="imgSlide slide_2"></div>
            </swiper-slide>
            <swiper-slide>
                <div class="imgSlide slide_3"></div>
            </swiper-slide>
            <swiper-slide>
                <div class="imgSlide slide_4"></div>
            </swiper-slide>
        </swiper>
        </div>
        <div class="content">
            <h2>Galerie</h2>
            <p>Nous travaillons avec des <strong>modeles</strong> de tous types et de tous âges.Que vous cherchiez des mannequins pour des <strong>defiles de mode</strong>, des séances photos, des publicités, des vidéos ou des <strong>evenements spéciaux</strong>, nous avons les meilleurs talents pour vous aider à atteindre vos objectifs.</p>
            <p class="last-child">Nous nous engageons à aider nos mannequins à se <strong>developper dans leur carriere</strong>, en leur offrant une formation et des conseils personnalisés pour améliorer leur <strong>technique</strong> de marche, leur posture, leur expression faciale, leur pose et leur style.</p>
            <a class="btn green" href="">Visitez</a>
        </div>
    </section>

    <section id="services">
        <div class="content">
            <h3>Nos services</h3>
            <p>
                Si vous cherchez à devenir mannequin ou à travailler avec les meilleurs <strong>talents de Paris</strong>, notre agence de mannequin est l'endroit idéal pour commencer. <strong>Contactez-nous</strong> dès maintenant pour en savoir plus sur nos services et pour commencer votre voyage dans l'industrie de la mode.
            </p>
            <a href="">Visitez</a>
        </div>
        <div class="services">

        </div>
    </section>
</template>

<script>

    import { Pagination } from 'swiper';
    // Import Swiper Vue.js components
    import { Swiper, SwiperSlide } from 'swiper/vue';
    // Import Swiper styles
    import 'swiper/css';
    import 'swiper/css/pagination';

    export default {
        components: {
            Swiper,
            SwiperSlide,
        },
        setup() {
            const onSwiper = (swiper) => {
            console.log(swiper);
            };
            const onSlideChange = () => {
            console.log('slide change');
            };
            return {
            onSwiper,
            onSlideChange,
            modules: [Pagination],
            };
        },
    };
</script>