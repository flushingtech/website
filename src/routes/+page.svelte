<script>
    import '../app.css';
    import Main from './Main.svelte';
    import Nav from './Nav.svelte'
    import Carousel from '../components/Carousel.svelte';
    import Events from '../components/Events.svelte'
</script>

<Nav></Nav>
<Main></Main>
<Carousel></Carousel>
<Events></Events>


<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        width: 80%;
        margin: auto;
    }
</style>
