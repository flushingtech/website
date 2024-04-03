<script>
    import '../app.css';
    import Event from './Event.svelte';
    import Main from './Main.svelte';
    import Profolio from './Profolio.svelte';
    import Nav from './Nav.svelte'
</script>

<Nav></Nav>
<Main></Main>
<Event></Event>

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
