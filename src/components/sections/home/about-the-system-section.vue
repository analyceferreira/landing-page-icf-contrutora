<script setup>
    import CheckSolidIcon from '/src/components/icons/icon-check-solid-svg.vue'
</script>


<template>
<section class="">
    <div class=" about-the-sytem-container container">
    <div class="about-divider image">
        <img class="image-principal" 
        src="/src/assets/images/certifield-builder-iforms.png" alt="imagem de uma placa de iforms branca com simbolo de certificado escrito Certifield Builder IForms em um fundo verde">
        <img class="image-element" 
        src="/src/assets/images/certifield-builder-iforms-element.png" alt="Elemento decorativo verde com bordas arredondadas">
    </div>
    <div class="about-divider infos">
        <div>
            <h3>Conheça mais sobre</h3>
            <h2>O sistema construtivo IForms</h2>
        </div>
        <p>Um sistema inteligente formado por formas de EPS tipo lego que não propaga chamas que é preenchido com aço e concreto, formando uma parede de concreto armado que funciona como vedação e estrutural em simultâneo.</p>

        <div class="checks">
            <CheckSolidIcon/>
            <span>Rápido e Prático</span>
        </div>
        <div class="checks">
            <CheckSolidIcon/>
            <span>Eficiênte E Econômico</span>
        </div>
        <div class="checks">
            <CheckSolidIcon/>
            <span>Sustentável</span>
        </div>
        
        <a href="https://www.iforms.com.br"><button>Saiba mais</button></a>
    </div>
    </div>

</section>
</template>



<style>
.about-the-sytem-container {
    display: flex;
    gap: 3%;
}

.about-divider {
    width: 50%;
}

.about-divider.image {
    width: 60%;
}

.image .image-principal {
    width: 100%;
    position: relative;
    transition: all .3s ease-in-out;
    animation: particlemove2 4.5s infinite linear;
}
@keyframes particlemove2 {
  0% {
    transform: translate(0, 0);
    -webkit-transform: translate(0, 0);
  }

  25% {
    transform: translate(10px, 10px);
    -webkit-transform: translate(10px, 10px);
  }

  50% {
    transform: translate(5px, 5px);
    -webkit-transform: translate(5px, 5px);
  }

  75% {
    transform: translate(10px, -5px);
    -webkit-transform: translate(10px, -5px);
  }

  100% {
    transform: translate(0, 0);
    -webkit-transform: translate(0, 0);
  }
}

.image .image-element {
    width: 229px;

    position: absolute;
    left: 0;
    bottom: 0;
}

.about-divider.infos {
    display: flex;
    flex-direction: column;
    gap: 2em;
}

.checks {
    display: flex;
    gap: 1.5rem;
}

.checks span {
    font-size: var(--font-18px);
    font-family: var(--font-title-text);
    font-weight: var(--weight-bold);
    color: var(--color-title-text);
}

.checks svg {
    width: 1rem;
    opacity: 70%;
    fill: var(--color-text);
}


@media screen and (max-width: 850px) {
    .about-the-sytem-container {
        flex-direction: column;
    }

    .about-divider, .about-divider.image {
        width: 100%;
    }
}

@media screen and (max-width: 490px) {
    .image .image-element {
        width: 200px;

        position: absolute;
        left: 0;
        bottom: 0;
    }
}
</style>