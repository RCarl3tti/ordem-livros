<script lang="ts">
  export let autor: any = null;
</script>

{#if autor}
  <a
    href="/autores/{autor.id}"
    class="flex flex-col rounded-md relative overflow-hidden border border-zinc-800"
  >
    <img
      src={autor.imagem}
      alt="Foto do autor {autor.nome}"
      class="object-cover h-64"
    />
    <div class=" absolute bottom-0 px-6 py-4 bg-black/50 w-full flex justify-end">
        <span class="text-2xl font-black">{autor.nome}</span>
    </div>
  </a>
{/if}
