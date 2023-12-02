<script>
    import '../app.css';
    import Page from './+page.svelte';
    import Event from './Event.svelte';
    import Header from './Header.svelte';
    import LandingImage from './LandingImage.svelte';
</script>

<Header></Header>
<Page></Page>
<LandingImage></LandingImage>
<Event></Event>

<div class="container">
    <slot />
</div>

<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        width: 80%;
        margin: auto;
    }
</style>
