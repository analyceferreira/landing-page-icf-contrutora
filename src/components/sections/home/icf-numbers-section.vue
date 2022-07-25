<script setup>
  import IconGlobeSVG from '../../icons/icon-global-svg.vue'
  import IconFagSVG from '../../icons/icon-flag-svg.vue'
  import IconWallSVG from '../../icons/icon-deezer-svg.vue'
  import IconClockSVG from '../../icons/icon-clock-svg.vue'
</script>



<template>
<section class="numbers-icf">
    <div class="container">
    <div class="titles">
        <h3>A ICF Construtora</h3>
        <h2>A ICF Construtora em números</h2>
    </div>

    <div class="numbers-icf-cards">
        <div class="card">
            <div class="icon">
                <IconGlobeSVG/>
            </div>
            <div class="info">
                <h4>+ De 40 Licenciados</h4>
                <p>Licenciados são empresas que representam a marca da ICF Construtora em suas cidades.</p>
            </div>
        </div>
        <div class="card">
            <div class="icon">
                <IconFagSVG/>
            </div>
            <div class="info">
                <h4>+ De 500 Especialistas</h4>
                <p>Experts são especialistas em construção com iForms ICF, formados em nosso treinamento.</p>
            </div>
        </div>
        <div class="card">
            <div class="icon">
                <IconWallSVG/>
            </div>
            <div class="info">
                <h4>+ 150.000 M² De Parede</h4>
                <p>Já são mais de 150.000 m² de paredes iForms ICF construídas no Brasil.</p>
            </div>
        </div>
        <div class="card">
            <div class="icon">
                <IconClockSVG/>
            </div>
            <div class="info">
                <h4>Obras 40% Mais Rápidas Em Média</h4>
                <p>Obras executadas no sistema iForms ICF com a ICF Construtora tendem a ser 40% mais rápidas.</p>
            </div>
        </div>
    </div>
    </div>
    <img class="element" src="/src/assets/images/element-two-hero-page.png" alt="">

</section>
</template>



<style >
    .numbers-icf {
        top: 100px;
    }
    .numbers-icf .element {
        position: absolute;
        top: 0px;
        left: 0;
        width: 800px;

        z-index: 0;
    }
/*--------- Section ---------*/
.numbers-icf-titles {
    display: flex;
    flex-direction: column;
    align-items: center;
}



/*--------- Cards ---------*/
.numbers-icf-cards {
    display: flex;
    flex-wrap: wrap;

    gap: 3%;
    row-gap: 2em;
}

.card{
    width: 48.5%;
    padding: 2em 2.5em;
    border-radius: 10px;

    display: flex;
    gap: 2em;
    box-shadow: var(--shadow-card);
    background-color: var(--color-background);
}

.card .info {
    display: flex;
    flex-direction: column;
    gap: .7em;
}

/*--------- Cards hover ---------*/
.card:hover{
    background-color: var(--color-emphasis-text);
}
.card:hover p{
    color: var(--color-text-invert);
}

.card:hover h4{
    color: var(--color-background);
}



/* ---------- Responsive ajustments ------------ */

@media screen and (max-width: 760px) {
    .numbers-icf-cards {
        flex-direction: column;
    }

    .card{
        width: 100%;
    }
}

</style>