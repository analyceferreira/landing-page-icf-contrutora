<template>
<section >
    <div class="hero container">
        <div class="hero-info">
            <div>
                <h3>Conheça a</h3>
                <h1>ICF Construtora Inteligente</h1>
            </div>
            <p>Uma empresa especializada em construções com iForms ICF, um sistema construtivo inteligente, prático e rápido!</p>
            <a href="https://icfconstrutora.com.br/solicitar-orcamento/"><button>Solicitar orçamento</button></a>
        </div>
        <div class="iframe">
            <iframe allow="autoplay; fullscreen" type="text/html" src="https://www.youtube-nocookie.com/embed/Ska3K4OryH0?version=3&amp;enablejsapi=1&amp;html5=1&amp;volume=100&amp;hd=1&amp;wmode=opaque&amp;showinfo=0&amp;rel=0&amp;origin=https://icfconstrutora.com.br;&amp;controls=0&amp;playsinline=1" allowfullscreen width="100%" height="100%" class="intrinsic-ignore" style="opacity: 1; visibility: visible; width: 100%; height: 300px; display: block;" id="iframe83038" title="Conheça a ICF Construtora, especializada em construções com ICF (casas de ISOPOR)."></iframe>
        </div>
        <img class="element-one" src="/src/assets/images/element-hero-page.png" alt="">
        <img class="element" src="/src/assets/images/element-two-hero-page.png" alt="">
    </div>

</section>
</template>



<style>
    .hero .element {
        position: absolute;
        top: -100px;
        left: 0;

        z-index: 0;
    }
        .hero .element-one {
        position: absolute;
        top: -50px;
        left: -40px;

        z-index: 1;
    }
    /*------ Hero section ------*/
    .hero {
        display: flex;
        gap: 2%;
        width: 100%;
        position: static;
    }

    .hero div {
        width: 100%;
    }


    /*------ Hero Infos ------*/
    .hero-info {
        display: flex;
        flex-direction: column;

        gap: 3em;
    }

    .hero-info h3 {
        color: var(--color-soft-text);
    }

    h1 {
        color: var(--color-emphasis-text);
        font-size: 2.44rem;
        font-weight: var(--weight-extra-bold);
        font-family: var(--font-title-text);
        letter-spacing: -0.01rem;
    }

    .hero button {
        background: var(--color-gradient-soft);
        margin-bottom: .1em;
    }


    /*------ Hero video ------*/

    
    .hero iframe {
        width: 100%;
        border-radius: 20px;
        padding: 0;
    }



    @media screen and (max-width: 870px) {
        .hero {
            flex-direction: column;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        h1 {
            color: var(--color-emphasis-text);
            font-size: var(--font-30px);
            margin-bottom: .5em;
        }

        .hero button {
            position: absolute;
            bottom: -22em;
        }
        .hero-info {
            gap: 0;
        }
    }

</style>