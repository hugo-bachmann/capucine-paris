<template>
    <section id="accueil" class="container section">
        <h1>Grapucine</h1>
        <p>paris</p>
        <a class="btn" href="/#contact">Visitez</a>
        <span class="modelName">Model : Abir Hamdi</span>
    </section>

    <section id="notre-histoire" class="section">
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
    
    <section id="galerie" class="section">
        <div class="slider">
            <swiper
            :slides-per-view="1"
            :space-between="0"
            :pagination="true"
            :modules="modules"
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

    <section id="services" class="section">
        <div class="content">
            <h3>Nos Services</h3>
            <p>
                Si vous cherchez à devenir mannequin ou à travailler avec les meilleurs <strong>talents de Paris</strong>, notre agence de mannequin est l'endroit idéal pour commencer. <strong>Contactez-nous</strong> dès maintenant pour en savoir plus sur nos services et pour commencer votre voyage dans l'industrie de la mode.
            </p>
            <a class="btn green" href="">Visitez</a>
        </div>
        <div class="services">
            <swiper
            :slides-per-view="3"
            :space-between="0"
            :loop="true"
            :modules="modules"
            >
                <swiper-slide>
                    <div class="service green">
                        <!-- <span>Text on path</span> -->
                        <h4>PHOTOGRAPHIE</h4>
                        <a class="btn" href="">Visitez</a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="service orange">
                        <!-- <span>Text on path</span> -->
                        <h4>PHOTOGRAPHIE</h4>
                        <a class="btn" href="">Visitez</a>
                    </div>
                </swiper-slide>
                <swiper-slide>
                    <div class="service grey">
                        <!-- <span>Text on path</span> -->
                        <h4>PHOTOGRAPHIE</h4>
                        <a class="btn" href="">Visitez</a>
                    </div> 
                </swiper-slide>
            </swiper>
        </div>  
    </section>

    <section id="contact" class="section">
        <div class="form">
            <h3>Nous rejoindre</h3>
            <form action="">
                <div class="dual">
                    <div class="inputContainer">
                        <label for="prenom">Prenom</label>
                        <input type="text" id="prenom" name="prenom" placeholder="Mathilde">
                    </div>
                    <div class="inputContainer">
                        <label for="nom">Nom</label>
                        <input type="text" id="nom" name="nom" placeholder="Jaus">
                    </div>
                </div>
                <div class="inputContainer">
                    <label for="email">Adresse Mail</label>
                    <input type="text" id="email" name="email" placeholder="mathildejaus@gmail.com">
                </div>
                <div class="inputContainer">
                    <label for="telephone">Numero de Telephone</label>
                    <input type="tel" id="telephone" name="telephone" placeholder="+33 6 XX XX XX XX">
                </div>
                <div class="inputContainer">
                    <label for="objet">Objet</label>
                    <input type="text" id="objet" name="objet" placeholder="Candidature Mlle Jaus">
                </div>
                <button class="btn" type="submit">Etre contacte</button>
            </form>
        </div>
        <div class="imgContainer">

        </div>
        <div class="contact">
            <h3>Nous contacter</h3>
            <p>Capucine Paris</p>
            <p>16 Rue de la Pompe, 75016 Paris, France</p>
            <p>+33 1 45 24 78 90</p>
            <p>contact@parischicmodels.com</p>
        </div>
    </section>
</template>

<script>
    import { Swiper, SwiperSlide } from 'swiper/vue';
    // Import Swiper styles
    import 'swiper/css';
    import 'swiper/css/pagination';

    import { Pagination } from 'swiper';


    export default {

        components: {
            Swiper,
            SwiperSlide,
        },
        setup() {
            return {
                pagination: {
                    clickable: true,
                },
                modules: [Pagination],
            };
        },
    };
</script>