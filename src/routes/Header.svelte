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

<div class = 'top'>
    <div class = "title">
        <h1>Flushing Tech's Hackathon Group</h1>

    </div>
    
    <LandingImage></LandingImage>
</div>
<div class= "description">
    Join our freeform, self-organized hackathons where creativity knows no bounds. Whether you're a seasoned pro, aspiring entrepeneur, or passionate hobbyist, our events are tailor-made for tech enthusiasts like you. Bring a laptop, your brightest ideas, and ongoing projects - lets build something together! 
</div>



<style>

    .title {
        font-weight: bold;
        font-size: 3.5rem;
        margin-bottom: .5rem;
        display: flex;
        justify-content: center;
        align-items: center;
        color:rgba(255, 255, 255, 0.925);
    }

    .top{
        display: flex;
        justify-content: space-around;
        /* border-width: 2px; */
        margin-left: 1.5rem;
        margin-right: 1.5rem;
        margin-top: 1rem;
        margin-bottom: 2rem;

    }

    .description{
        margin-left: 2.5rem;
        margin-right: 2.5rem;
        margin-top: 1rem;
        margin-bottom: 2rem;
        text-align: center;
        color:rgba(255, 255, 255, 0.85);
        /* border-width: 2px; */
    }


</style>