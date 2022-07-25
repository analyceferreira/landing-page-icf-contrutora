<script setup> 
    import WaveSvg from '../../icons/wave-svg.vue'
</script>

<template>
<section class="group-icf section-gradient">
    <WaveSvg/> 
    <div class="group-icf-container">
        <div class="image">
            <img src="/src/assets/images/grupo.icf.png" alt="">
        </div>
        <div class="infos">
            <h2>A ICF Construtora é o ramo de execução de obras do Grupo ICF</h2>
            <p>O Grupo ICF é a união de diversas empresas sob um objetivo comum: o de conferir mais agilidade, eficiência, segurança, renda e economia quem trabalha com o sistema iForms ICF e para quem mora em empreendimentos e residências construídas com o sistema.</p>

            <a href="https://grupoicf.com.br"> <button>Saiba mais</button> </a>
        </div>
    </div>
</section>
</template>


<style>
section.group-icf {
    margin-top: -5%;
    padding-top: 18%;
}
.group-icf-container {
    width: 100%;
    display: flex;
    gap: .5%;
}

.group-icf-container .image {
    width: 53%;
    transition: 0.3s;
    right: 0;
}

.group-icf-container .image:hover {
    right: 10px;
}


.group-icf-container img {
    width: 100%;
    object-fit: contain;
}


.group-icf-container .infos {
    width: 50%;

    margin-top: .5em;
    display: flex;
    flex-direction: column;
    gap: 2em;
}


@media screen and (max-width: 950px) {
    .group-icf-container {
        flex-direction: column;
    }

    .group-icf-container .infos, .group-icf-container .image {
        width: 100%;
    } 
}
</style>