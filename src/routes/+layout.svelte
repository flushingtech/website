<script>
    import '../app.css';
    import Header from './Header.svelte';
</script>

<Header></Header>

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