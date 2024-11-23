<script>
    import ItemAutor from "../../components/autor/ItemAutor.svelte";
    import autores from "../../constantes/autores.js";
    import Titulo from "../../shared/Titulo.svelte";
</script>

<dir class="flex flex-col gap-10">
    <Titulo
        principal="Autores"
        secundario="Conheça os autores que escreveram as histórias que você ama"
    />

    <div class="grid grid-cols-2 gap-5">
        {#each autores as autor}
            <ItemAutor {autor} />
        {/each}
    </div>
</dir>
