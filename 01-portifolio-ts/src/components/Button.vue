<script lang="ts">
export default {
    props: {
        texto: String,
        endereco: String,
    }
}
</script>
<template>
<!-- https://www.instagram.com/leirisson99/
https://github.com/leirisson -->

    <button class="btb-redes-btn">
        <a :href="endereco">
            {{ texto }}
        </a>
    </button>

</template>


<style scoped>
.btb-redes-btn {
    padding: 1rem;
    border: none;
    width: 40%;
    gap: 1rem;
    color: var(--preto);
    background: var(--azul-claro);
    font-weight: 600;
    border-radius: 1rem;
    transition: color .1s;
    font-family: "Krona One", serif;
}

.btb-redes-btn:hover {
    background: var(--azul-hover);
}
a{
    text-decoration: none;
    color: var(--preto);
}
</style>