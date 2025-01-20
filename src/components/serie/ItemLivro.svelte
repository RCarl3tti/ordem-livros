<script lang="ts">
  import { IconBrandAmazon } from '@tabler/icons-svelte';
  export let livro: any = null;
</script>

{#if livro}
  <a href={livro.link} target="_blank" class="flex flex-col rounded-md overflow-hidden bg-zinc-800">
    <img src={livro.imagem} alt="Capa do livro {livro.titulo}" class="max-h-96"/>
    <div class="flex-1 flex flex-col p-5 gap-2">
      <span class="flex-1 font-bold">{livro.titulo}</span>
      <button class="botao azul"> 
          <IconBrandAmazon size={25}/>
          <span>Link do Livro</span> 
         </button>
    </div>
  </a>
{/if}
