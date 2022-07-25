<template>
<section class="aks-quote">
    <div class="aks-quote-container">
        <div>
            <h2>Solicite um orçamento</h2>
            <p>Nós atendemos todo o Brasil com nossos Licenciados e Experts, converse com nossos especialistas via WhatsApp, eles te ajudarão a localizar o seu representante.</p>
        </div>

        <a href="https://icfconstrutora.com.br/solicitar-orcamento/"><button>ORÇAMETO</button></a>
    </div>
</section>
</template>


<style>
section.aks-quote {
    margin: var(--section-gap) 0;
    padding: 7% 2%;
    background: var(--color-gradient-dark);
}

.aks-quote-container {
    width: 100%;
    height: 120px;
    margin: none;

    display: flex;
    align-items: center;
    gap: 2%;
}

.aks-quote-container h2 {
    margin-bottom: .3em;
}

.aks-quote-container h2, .aks-quote-container p {
    color: var(--color-background);
}

.aks-quote-container button {
    background: var(--color-background);
    color: var(--color-mute-text);
    height: 100%;
}




@media screen and (max-width: 1025px) {
    .aks-quote-container {
        flex-direction: column;
        text-align: center;
        align-items: center;
        justify-content: center;
        height: 170px;

    }

    .aks-quote-container p {
        margin: 0 5%;
    }

    .aks-quote-container h2, .aks-quote-container p {
            margin-bottom: .5em;
    }

    .aks-quote-container button {
        width: 250px;
    }
}



@media screen and (max-width: 770px) {
    .aks-quote-container {
        margin: .5em 0 2em;
        text-align: start;
        align-items: flex-start;
        height: 100%;
    }

    .aks-quote-container p {
        margin: 0 0 1em 0;
    }

    .aks-quote-container h2 {
        margin-bottom: 0em;
    }

    .aks-quote-container a {
        width: 100%;
    }

    .aks-quote-container a button {
        width: 100%;
    }
}
</style>