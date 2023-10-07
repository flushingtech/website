<script>
    import '../app.css';
    import Header from './Header.svelte';
</script>

<Header></Header>
<slot class="container" />

<style>
    .container {
        display: flex;
    }
</style>