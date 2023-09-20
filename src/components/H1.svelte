<script>
    let styles=$$props.style
</script>

<h1 style={styles}>
    <slot />
</h1>

<style>
    h1 {
        font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
        font-size: clamp(2rem, 4vw, 5rem);
        text-align: center;
        color: var(--primarycolor);
    }
</style>