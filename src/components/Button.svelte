<script>
    let styles=$$props.style;
    export let handleClick = () => alert('Please pass a function through the props');
</script>

<button on:click={handleClick} style={styles}>
    <slot />
</button>


<style>
    button {
        font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
        font-weight: 500;
        font-size: 24px;
        padding-inline: 15px;
        padding-block: 5px;
        border-radius: 10px;
        border: 2px solid;
        border-color: var(--primarycolor);
        background-color: 'transparent';
        color: var(--primarycolor);
        cursor: pointer;
        transition: all ease-in-out 0.3s;
    }
    button:hover {
        color: #ffffff;
        background-color: var(--primarycolor);
    }
    button:active {
        transform: translateY(1px);
        transition: all ease 0.1s;
    }
</style>