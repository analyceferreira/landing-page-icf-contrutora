<script setup>
    import CheckIcon from '../../icons/icon-check-svg.vue'
    import ExclationIcon from '../../icons/icon-exclamation-svg.vue'
    import WhatsappIcon from '../../icons/icon-whatsapp-svg.vue'
    import MoneyCardIcon from '../../icons/icon-money-svg.vue'
    import Radcon from '../../icons/icon-graduation-svg.vue'
    import MedalIcon from '../../icons/icon-medal-svg.vue'
</script>



<template>
<section class="about-icf">
    <div class="container">
    <div class="about-icf-titles">
        <h3>Conheça mais sobre</h3>
        <h2>Como construir com a ICF Construtora</h2>
    </div>

    <div class="about-icf-cards">
        <div class="collumn one">
            <div class="card move-right">
                <div class="icon">
                    <CheckIcon/>
                </div>
                <div class="info">
                    <h4>Já Tem Projeto?</h4>
                    <p>Localize o representante mais próximo e envie o projeto para o orçamento</p>
                </div>
            </div>
            <div class="card">
                <div class="icon">
                    <ExclationIcon/>
                </div>
                <div class="info">
                    <h4>Não Tem Projeto?</h4>
                    <p>Envie uma solicitação de projeto para a ICF Projetos</p>
                </div>
            </div>
            <div class="card move-right">
                <div class="icon">
                    <WhatsappIcon/>
                </div>
                <div class="info">
                    <h4>Não Localizou O Representante?</h4>
                    <p>Nós chame no Whats para te auxiliar</p>
                </div>
            </div>
        </div>
        <div class="collumn two">
            <img src="/src/assets/images/icf-construtora-sede.png" alt="">
        </div>
        <div class="collumn">
            <div class="card move-left">
                <div class="icon">
                    <MoneyCardIcon/>
                </div>
                <div class="info">
                    <h4>Precisa De Financiamento?</h4>
                    <p>Possuímos parceria com a plataforma Minha Casa Financiada.</p>
                </div>
            </div>
            <div class="card">
                <div class="icon">
                    <Radcon/>
                </div>
                <div class="info">
                    <h4>Construa Você Mesmo!</h4>
                    <p>Se torne um Expert em iForms ICF com nossa formação</p>
                </div>
            </div>
            <div class="card move-left">
                <div class="icon">
                    <MedalIcon/>
                </div>
                <div class="info">
                    <h4>Já Conhece O ICFlex?</h4>
                    <p>Acabamento 5 em 1 que elimina chapisco e reboco.</p>
                </div>
            </div>
        </div>
    </div>
    </div>
</section>
</template>


<style>
.about-icf {
    display: flex;
    flex-direction: column;
    gap: 3.5em;
}
.about-icf-titles {
    display: flex;
    flex-direction: column;
    align-items: center;
}



.about-icf-cards {
    display: flex;
    position: relative;
    justify-content: space-between;
}

.about-icf-cards .collumn {
    width: 30%;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: .5em;

    position: relative;
}

.about-icf-cards .collumn.one {
    justify-content: space-between;
    position: 5;
}

.about-icf-cards .collumn.two {
    margin: -10px;
    position: 1;
}

.collumn .card {
    width: 100%;
    padding: 1em 1.5em;
}

.about-icf-cards .collumn img {
    width: 380px;
}

.card.move-right {
    right: -2em;
}

.card.move-left {
    left: -2em;
}


@media screen and (max-width: 1050px) {
    .about-icf-cards {
        flex-direction: column;
        gap: 2em;    
    }

    .about-icf-cards .collumn {
        width: 100%;
    }

    .card.move-right, .card.move-left {
        left: 0;
        right: 0;
    }

    .about-icf-cards .collumn.two {
        margin: 0;
    }

    .collumn .card {
        padding: 1.5em 4%;
    }
}

</style>