<script>
    import Logo from './Logo.svelte';
    import Search from './Search.svelte';
</script>

<div class="navigation">
    <Logo></Logo>
    <div class="brand-text">Flushing Tech</div>
    <Search></Search>
</div>

<style>
    .navigation {
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        display: flex;
        flex-direction: row;
        background-color: #eaeaea;
        padding: 0;
    }


    .brand-text {
        font-weight: bold;
        font-size: 2rem;
    }
</style>