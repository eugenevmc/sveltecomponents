<script>
    let styles=$$props.style;
    export let type = 'regular'; //regular or metallic 
</script>

{#if type == 'metallic'}
    <header style={styles} class='metallic'>
        <slot />
    </header>
{:else}
    <header style={styles}>
        <slot />
    </header>
{/if}

<style>
    header {
        font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
        font-weight: 700;
        font-size: 120px;
        text-align: center;
        color: var(--primarycolor);
    }

    @media screen and (max-width : 1200px) {
        header {
            font-size: 100px;
        }
    }

    @media screen and (max-width: 768px) {
        header {
        font-size: 75px;
        }
    }
    header.metallic {
        background: linear-gradient(185deg, #848789, 40%,
        #d1d5db, #e5e7eb, 65%, #848789);
        -webkit-text-fill-color: transparent;
        -webkit-background-clip: text;
        background-clip: text;
    }
</style>