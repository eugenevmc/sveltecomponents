<header>
    <slot />
</header>

<style>
    header {
        font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
        font-weight: 700;
        font-size: 120px;
        text-align: center;
        color: var(--color);
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
</style>