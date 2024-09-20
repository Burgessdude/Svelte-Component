<script>
	export let name = "Default";
	export let type = "regular"; // regular, flat, disabled
	export let size = "md"; // sm, md, lg
	const sizes = {
		"sm" : "px-1 py-3 pr-8 pl-8",
		"md" : "px-5 py-3 pr-8 pl-4",
		"lg" : "px-7 py-5 pr-8 pl-8",
	}
</script>

{#if type=="regular"}
 <button class={`text-black border-2 border-blue-700 font-medium h-12 w-80 rounded-xl text-left align-middle ${(size in sizes) ? sizes[size] : sizes["md"]}`}>
  {name}
 </button>
{/if}

{#if type=="flat"}
 <button class={`text-slate-50 border-2 border-gray-300 h-12 w-80 rounded-xl text-left align-middle ${(size in sizes) ? sizes[size] : sizes["md"]}`}>
  {name}
 </button>
{/if}

{#if type=="disabled"}
 <button class={`text-black border-2 border-red-700 font-medium h-12 w-80 rounded-xl text-left align-middle ${(size in sizes) ? sizes[size] : sizes["md"]}`}>
  {name}
 </button> 
{/if}

{#if type=="fourth"}
 <button class={`text-black border-2 border-gray-300 h-12 w-80 rounded-xl text-left align-middle ${(size in sizes) ? sizes[size] : sizes["md"]}`}>
  {name}
 </button>
{/if}

{#if type=="fifth"}
 <button class={`bg-gray-300 text-gray-400 border-2 border-gray-200 h-12 w-80 rounded-xl text-left align-middle ${(size in sizes) ? sizes[size] : sizes["md"]}`}>
  {name}
 </button>
{/if}