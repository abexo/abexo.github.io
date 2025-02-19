<script lang="ts">
    import { CardItem, CardSkillItem }  from '$lib';

    let { 
        data, 
        title = null, 
        bgTitle = "#b1e82e", 
        animationClasses,
        titleColor = "white",
        rotateTitle = "-rotate-3",
        type = "default" // single, defailt, static, image
    } = $props();

</script>

<div class="overflow-hidden">
<div class={`flex flex-col flex-grow mt-10 brb bg-[#090516] border-dashed rounded-2xl border-[#ffffff4f] px-5 py-6 ${animationClasses}`}>
    <div class={`mx-auto max-w-max -mt-11 ${rotateTitle}`}>
        <h2 class="animate__animated animate__rubberBand animate__delay-2s font-medium text-xl text-center w-auto px-4 py-1 rounded-lg" style={`background-color: ${bgTitle}; color: ${titleColor}`}>{title}</h2>
    </div>
    <ul class={`${type === "single" ? "pt-7 flex flex-wrap space-x-2 space-y-1" : "pt-7"}`}>
        {#if type === "single"}
            {#each data as item}
                <CardSkillItem {item}/>
            {/each}        
        {:else if type === "static"}
            <div class="flex">
                <p class="flex-1 font-light text-xs">
                    Got a cool project? I’m more than happy to help, reach out anytime! I’m always open to contribute, or just chat about ideas.
                </p>
            </div>
        {:else if type === "image"}
            <div class="flex flex-wrap space-x-2 justify-around space-y-1">
                {#each data as item}
                   <img class="object-cover" src="{item.link}" alt="logo">
                {/each}
            </div>
        {:else}
            {#each data as item}
                <CardItem {item}/>
            {/each}
        {/if}
    </ul>
</div>
</div>