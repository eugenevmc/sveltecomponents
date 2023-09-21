<script lang='ts'>
    import Header from "../components/Header.svelte"
    import H1 from "../components/H1.svelte"
    import Button from "../components/Button.svelte"
</script>

<body style="
display: flex; 
flex-direction: column;
justify-content:center;
align-items: center;
gap: 5px;
height: 80vh;
">
    <Header type=metallic>VISta</Header>
    <H1>Welcome to the new Vista Information System!</H1>
    <p style="display: flex;">
        this is my p tag
    </p>
    <Button --primarycolor=#172554>Button</Button>
    <Button --primarycolor=#172554 handleClick={() => alert('Testing 123')}>Button2</Button>
</body>

<style>
    :root {
        --primarycolor: #848789
    }
</style>