<script setup>
    import FacebookIcon from '/src/components/icons/icon-facebook-svg.vue'
    import InstagramIcon from '/src/components/icons/icon-instagram-svg.vue'
    import TelegramIcon from '/src/components/icons/icon-telegram-svg.vue'
    import YouTubeIcon from '/src/components/icons/icon-youtube-svg.vue'
</script>


<template>
<section class="footer">
    <div class="footer-buttons">
        <div class="collumn one">
            <img src="/src/assets/images/ICF-Construtora-logo.png" alt="">
            <div>
                <p>Uma empresa especializada em construções com ICF (o famoso isopor) ou EPS.</p>
                <div class="icons">
                    <a href="http://" class="icon"><FacebookIcon/></a>
                    <a href="http://" class="icon"><InstagramIcon/></a>
                    <a href="http://" class="icon"><YouTubeIcon/></a>
                    <a href="http://" class="icon"><TelegramIcon/></a>
                </div>
            </div>
        </div>
        <div class="collumn two">
            <h4>Atalhos</h4>
            <div>
                <a href="">Grupo ICF</a>
                <a href="">ICF Projetos</a>
                <a href="">ICF Argamassas</a>
            </div>
        </div>
        <div class="collumn two three">
            <h4>Contato</h4>
            <div>
                <button>WhasApp</button>
                <button>Orçamento</button>
            </div>
        </div>
    </div>
    <hr>
    <div class="footer-copyright">
        <p>2021 ICF Construtora Inteligente by <a target="_blank" href="https://ascensiondigital.com.br">Ascension Digital</a></p>
    </div>
</section>
</template>


<style>
.footer {
    width: 100%;
    height: 470px;
    background: var(--color-gradient-dark-2);
    margin-bottom: 0;
    padding-top: 10%;
    padding-bottom: 2%;

    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
.footer p, .footer h4, .footer a {
    color: var(--color-background)
}

.footer-buttons {
    display: flex;
    gap: 6%;
}

.footer-buttons .collumn {
    width: 30%;
    display: flex;
    flex-direction: column;
    gap: 1.5em;
}

.footer-buttons .collumn.one p {
    margin-bottom: .5em;
}

.footer-buttons .collumn.two {
    width: 26%;
    gap: 2em;
}

.footer-buttons .collumn.two div {
    display: flex;
    flex-direction: column;
    gap: .7em;
}

.footer-buttons .collumn.two button {
    width: 142px;
    padding: 0.6em 1.5em;

    background: var(--color-background);
    color: var(--color-mute-text);
}

.footer-buttons img {
    width: 150px;
}

.footer .icons {
    width: 100%;

    display: flex;
    gap: 1.6em;
}

.icons svg {
    width: 1.3rem;
    position: relative;
}

.icons a::before {
    content: "";
    width: 2.5rem;
    height: 2.5rem;

    border-radius: 50%;
    background: var(--color-background-mute);
    fill: var(--color-background);
    position: absolute;
    left: -10px;
    top: -9px;
}

.icons a{
    top: 5px;
    left: 9px;
}


.footer-copyright p, .footer-copyright a {
    text-align: center;
    font-size: var(--font-14px);
}


@media screen and (max-width: 750px) {
    .footer-buttons {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2em;
    }

    .footer-buttons .collumn {
        width: 100%;
        align-items: center;
        gap: 1.5em;
    }

    .footer .icons, .collumn div {
        justify-content: center;
        text-align: center;
    }

    .footer-buttons .collumn.three  {
        margin-bottom: 2em;
    }

    .footer {
        width: 100%;
        height: 100%;
    }

    .footer-copyright {
    padding: 2em 0 1em;
    }
}

</style>