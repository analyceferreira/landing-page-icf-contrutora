<script setup>
    import { ref } from 'vue';

    const open = ref(false)
    const links = [
        {name: 'Início', link: '#'},
        {name: 'Licenciados', link: '#licenseds'},
        {name: 'Experts', link: '#experts'},
        {name: 'Obras', link: '#ours-constructions'},
        {name: 'Calculadora', link: 'https://icfconstrutora.com.br/calculadora/'},
        {name: 'Orçamento', link: 'https://icfconstrutora.com.br/solicitar-orcamento/'},
        {name: 'Trabalhe Conosco', link: 'https://docs.google.com/forms/d/e/1FAIpQLSfA7wjh_id4fqTQbIcIxUWVnQOCPDeQlIJlkPv8jOagOUstOA/viewform'}
    ]

    function MenuOpen() {
        open.value = !open.value
    }

</script>


<template>
    <header>
        <div>
            <a href="#"><img src="https://icfconstrutora.com.br/wp-content/uploads/2020/10/LADO-VERDE-FUNDO-BRANCO.png" alt="Logo ICF reduzida cor verde fundo"></a>
        </div>
        <nav :class="[open? '' : 'hidden']">
            <a v-for="link in links" :href="link.link">{{link.name}}</a>
        </nav>
        
        <div class="menu-hamburger">
            <label for="check">
                <input type="checkbox" @click="MenuOpen()"  id="check"/> 
                <span></span>
                <span></span>
                <span></span>
            </label>
        </div>

    </header>
</template>




<style scoped>
    header {
        background-color: var(--color-background);
        height: 100px;
        width: 100%;
        padding: var(--margin-global);

        display: flex;
        justify-content: space-between;
        align-items: center;

        box-shadow: 8px 3px 30px 5px var(--color-shadow);
        z-index: 5;
    }

    img {
        height: 4rem;
        z-index: 5;
    }

    nav {
        display: flex;
        gap: 1rem;
    }

    a {
        color: var(--color-title-text);
        font-weight: var(--weight-soft-bold);
        font-family: var(--font-title-text);
        font-size: 1.06rem;
    }
    
    .menu-hamburger {
        visibility: hidden;
        font-size: 1.5em;
        font-weight: var(--weight-bold);
        position: absolute;
        right: 5%;
        top: 1.5em;
    }

    label{
        display:flex;
        flex-direction:column;
        align-items: end;
        width:25px;
        cursor:pointer;
    }

    label span{
        background: var(--color-title-text);
        border-radius:10px;
        height:3px;
        margin: 3px 0;
        transition: .4s  cubic-bezier(0.68, -0.6, 0.32, 1.6);
    }


    span:nth-of-type(1){
        width:100%;  
    }

    span:nth-of-type(2){
        width:100%;
    }

    span:nth-of-type(3){
        width:100%;
    }


    input[type="checkbox"]{
        display:none;
    }


    input[type="checkbox"]:checked ~ span:nth-of-type(1){
        transform-origin:bottom;
        transform:rotatez(45deg) translate(7px,5px)
    }


    input[type="checkbox"]:checked ~ span:nth-of-type(2){
        transform-origin:top;
        transform:rotatez(-45deg);

    }


    input[type="checkbox"]:checked ~ span:nth-of-type(3){
        transform-origin:bottom;
        width:0%;
        transform: translate(-1px,-4.5px) rotatez(45deg);
    }




    @media screen and (max-width: 950px) {
        header {
            background-color: var(--color-background);
            height: 100px;
            width: 100%;
            padding: var(--margin-global);
            padding-top: 1em;

            flex-direction: column;

            justify-content: flex-start;
            align-items: flex-start;
            position: relative;            
        }
        nav {
            width: 100%;
            height: 100vh;
            margin-top: 5em;
            padding-top: 1em;
            padding-left: 1em;

            flex-direction: column;
            gap: .5rem;
            position: absolute;
            z-index: 5;
            background-color: var(--color-background);
        }

        .hidden {
            left: -120%;
        }

        .menu-hamburger {
            visibility: visible;
        }
    }
</style>