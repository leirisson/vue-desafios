<script lang="ts">
import Button from './Button.vue'
import Imagem from './Imagem.vue'

export default {
    
    components: {
        Button,
        Imagem,

    }
}
</script>

<template>
    <main class="container">
        <div class="conteudo_principal">
            <h1 class="conteudo_principal-texto">
                Eleve seu negócio digital a outro nível <span class="tituloAzul">com um Front-end de qualidade!</span>
            </h1>
            <p class="text">Olá! Sou Leirisson Souza, desenvolvedora Front-end com especialidade em React, HTML e CSS. Ajudo pequenos
                negócios e designers a colocarem em prática boas ideias. Vamos conversar?
            </p>
            <div class="btb-redes">
                <Button texto="Instagram"/>
                <Button texto="GitHub"/>
            </div>
        </div>
        <div class="img_perfil">
            <Imagem />
        </div>
    </main>

</template>

<style scoped>
.container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 1rem;
    width: 55rem;
    padding: 1rem;
    margin: 10rem auto;
    border-radius: 4px;
    border: 2px solid var(--azul-claro);
    line-height: 1.2;
}
.conteudo_principal-texto{
    font-size: 2rem;
    margin-bottom: 1rem;
    font-family:  "Krona One", serif;
}
.tituloAzul{
    color: var(--azul-claro);
}

.text{
    line-height: 1;
    margin-bottom: 1rem;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
   
}
.btb-redes{
    display: flex;
    width: 80%;
    justify-content: space-evenly;
    padding: 1rem;
    margin: 1rem auto;
}



</style>