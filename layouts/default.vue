<script>
    export default {
        methods: {
            toggleMenu() {
                const menu = document.querySelector ('#menu')
                menu.classList.toggle ('hiddenMobile')

                const burger = document.querySelector ('.burger')
                burger.classList.toggle ('active')
            },
        },
    }
</script>

<template>
    <header id="header">
        <nav id="menu" class="hiddenMobile">
            <ul>
                <li>
                    <a href="/">Accueil</a>
                </li>
                <li>
                    <a href="/">Notre histoire</a>
                </li>
                <li>
                    <a href="/">Galerie</a>
                </li>
                <li>
                    <a href="/">Services</a>
                </li>
                <li>
                    <a href="/">Contact</a>
                </li>
            </ul>
        </nav>

        <div class="burger" @click="toggleMenu">
            <div></div>
        </div>

    </header>

    <main id="body">
        <slot />
    </main>

</template>
