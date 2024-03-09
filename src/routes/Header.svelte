<script>
    import Logo from './Logo.svelte';
    import Search from './Search.svelte';
    import LandingImage from './LandingImage.svelte';
</script>

<!-- <div class="navigation">
    <Logo></Logo>
    <div class = "center-nav">
        <div>About</div>
        <div>Projects</div>
        <div>Members</div>
    </div>
    <Search></Search>
</div> -->

<div class = 'nav'>
    <h1 class="brand-text">Flushing Tech's Official Hackathon</h1>
    <LandingImage></LandingImage>
</div>

<style>
    /* .navigation {
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        display: flex;
        flex-direction: row;
        background-color: #8f6232;
        padding: 0;
        align-items: center;
        justify-content: space-between;
    } */


    .brand-text {
        font-weight: bold;
        font-size: 3.5rem;
        margin: 0 0.5rem;
    }

    .nav{
        display: flex;
        justify-content: space-between;
        border: 2px;
        border-color: black;
    }

    .intro{
        display: flex;
    }
</style>