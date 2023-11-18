<script>
    import '../app.css';
    import Header from './Header.svelte';
    import Profolio from './Profolio.svelte';
</script>

<Header></Header>

<div class="container">
    <slot />
</div>
<Profolio></Profolio>

<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        width: 80%;
        margin: auto;
    }
</style>
