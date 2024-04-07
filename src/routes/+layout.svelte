<script>
    import '../app.css';
    import Main from './Main.svelte';
    import Nav from './Nav.svelte'
    import Carousel from '../components/Carousel.svelte';
</script>

<Nav></Nav>
<Main></Main>
<Carousel></Carousel>


<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        width: 80%;
        margin: auto;
    }
</style>
