<script>
  import ItemAutor from "../../components/autor/itemAutor.svelte";
  import Titulo from "../../components/shared/Titulo.svelte";
  import autores from "../../constants/autores";
</script>


<div class="flex flex-col gap-5">
  <Titulo principal="Autores" secundario="Conheça os autores que escrevem as histórias que você ama" />
  
  <div class="grid grid-cols-2 gap-10">
      {#each autores as autor}
          <ItemAutor autor={autor} />
      {/each}
  </div>
</div>


