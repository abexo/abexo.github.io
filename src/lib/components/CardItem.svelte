<script>
    let { item } = $props();
</script>

<li class="item-m">
    {#if item.subtitle}
        <p class="text-[#afafae] text-xs font-extralight">{item.subtitle}</p>  
    {/if}
    <h3 class="font-semibold text-sm">{item.title}</h3>
    <p class="text-[#afafae] text-xs font-extralight">{item.description}</p>
</li>