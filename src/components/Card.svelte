<script>
    import {M} from 'svelte-motion';
    export let img;
    export let paragraph;
</script>

<M.div 
	initial={{scale: 1}}
	whileHover={{scale: 1.03}}
	transition={{duration:0.4}}
	class="w-[344px] border rounded-lg cursor-pointer">
		<img src={img} alt="{img} thumbnail" class="w-fit rounded-t-lg">
		<p class="px-1 sm:px-8 py-1 sm:py-4 text-xs md:text-sm">{paragraph}</p>
</M.div>