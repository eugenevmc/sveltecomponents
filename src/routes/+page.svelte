<script>
    import Header from "../components/Header.svelte"
    import H1 from "../components/H1.svelte"
    import Button from "../components/Button.svelte"
</script>

<body style="display: flex; 
flex-direction: column;
justify-content:center;
align-items: center;
">
    <Header --color='#172554'>VISta</Header>
    <H1>Welcome to the new Vista Information System!</H1>
    <Button --color='#172554'>Button</Button>
    <Button --color='#172554' handleClick={() => alert('Testing 123')}>Button2</Button>
</body>

<style>
    :root {
        --color: #848789
    }
</style>