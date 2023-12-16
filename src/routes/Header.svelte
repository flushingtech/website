<script>
    import Logo from "./Logo.svelte";
    import Search from "./Search.svelte";
    import LandingImage from "./LandingImage.svelte";
    import ModeSwitch from "./ModeSwitch.svelte";
</script>

<div class="navigation">
    <Logo></Logo>
    <div class="brand-text">Flushing Tech</div>
    <div class="ml-auto w-96">
        <Search></Search>
    </div>
    <div class="w-8"></div>
    <ModeSwitch></ModeSwitch>
    <div class="w-8"></div>

</div>

<style>
    .navigation {
        font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
        display: flex;
        flex-direction: row;
        background-color: #eaeaea;
        padding: 0;
        align-items: center;
    }

    .brand-text {
        font-weight: bold;
        font-size: 1.5rem;
        margin: 0 0.5rem;
    }
</style>
