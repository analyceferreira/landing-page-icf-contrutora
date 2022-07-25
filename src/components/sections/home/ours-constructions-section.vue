<script setup> 
    import WaveSvg from '../../icons/wave-svg.vue'
</script>


<template>
<section class="ours-construction section-gradient" id="ours-constructions">
    <WaveSvg/>

    <div class="titles">
        <h3>Conheça algumas de</h3>
        <h2>Nossas obras</h2>
        <p>Obras utilizando 100% o sistema iForms ICF</p>
    </div>

    <div class="contruction-cards">
        <a class="contruction-card" href="https://icfconstrutora.com.br/portfolio/sede-grupo-icf/">
            <img src="/src/assets/images/constructions/icf-sede.png" alt="">
            <div class="info">
                <h4>Sede Grupo ICF</h4>
                <span>Arquitetura Corporativa</span>
            </div>
        </a>
        <a class="contruction-card" href="https://icfconstrutora.com.br/portfolio/colegio-marista-sinop/">
            <img src="/src/assets/images/constructions/ifc-colegio-marista-sinop.png" alt="">
            <div class="info">
                <h4>Colégio Marista Sinop</h4>
                <span>Arquitetura Corporativa</span>
            </div>
        </a>
        <a class="contruction-card" href="https://icfconstrutora.com.br/portfolio/refeccs-sinop/">
            <img src="/src/assets/images/constructions/icf-reffecs.png" alt="">
            <div class="info">
                <h4>Refeccs Sinop</h4>
                <span>Arquitetura Corporativa</span>
            </div>
        </a>
        <a class="contruction-card" href="https://icfconstrutora.com.br/portfolio/apae-sinop/">
            <img src="/src/assets/images/constructions/icf-apae-sinop.png" alt="">
            <div class="info">
                <h4>Apae Sinop</h4>
                <span>Arquitetura Corporativa</span>
            </div>
        </a>
        <a class="contruction-card" href="https://icfconstrutora.com.br/portfolio/maple-bear-sorriso/">
            <img src="/src/assets/images/constructions/icf-mapple-bear.png" alt="">
            <div class="info">
                <h4>Maple Bear Sorriso</h4>
                <span>Arquitetura Corporativa</span>
            </div>
        </a>
        <a class="contruction-card" href="https://icfconstrutora.com.br/portfolio/banco-sicredi-sorriso/">
            <img src="/src/assets/images/constructions/icf-sicredi-sorriso.png" alt="">
            <div class="info">
                <h4>Banco Sicredi Sorriso</h4>
                <span>Arquitetura Corporativa</span>
            </div>
        </a>

    </div>
</section>
</template>


<style>
.ours-construction .titles {
    padding-top: 4%;
}
.contruction-cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    row-gap: 4.8em;
}

.contruction-card {
    display: flex;
    justify-content: center;
    width: 32%;
    position: relative;
}

.contruction-card img {
    width: 100%;
    border-radius: 5px;
    object-fit: contain;
}

.contruction-card .info {
    width: 85%;
    padding: .5em;
    text-align: center;

    background-color: var(--color-background);
    box-shadow: var(--shadow-card);
    border-radius: 5px;

    position: absolute;
    position: 5;
    bottom: -1.5em;
}
</style>