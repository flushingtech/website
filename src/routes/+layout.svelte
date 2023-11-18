<script>
    import '../app.css';
    import Header from './Header.svelte';
    import LandingImage from './LandingImage.svelte';
</script>

<Header></Header>

<div class="container">
    <slot />
</div>

<LandingImage></LandingImage>

<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        width: 80%;
        margin: auto;
    }
</style>
