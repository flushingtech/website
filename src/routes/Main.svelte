<script>
    import Logo from './Logo.svelte';
    import LandingImage from './LandingImage.svelte';
</script>

<div class = 'container'>
    <Logo></Logo>
    <LandingImage></LandingImage>

</div>

<div class="about-us-divider">
    <div class= "about-us-heading">
        What does this group do?
    </div>
    <div class= "about-us-text">
        We hold freeform, self-organized hackathons where creativity knows no bounds. Whether you're a seasoned pro, aspiring entrepeneur, or passionate hobbyist, our events are tailor-made for tech enthusiasts like you. Bring a laptop, your brightest ideas, and ongoing projects - lets build something together! 
    </div>

</div>

<!-- <div class= "description">
    Join our freeform, self-organized hackathons where creativity knows no bounds. Whether you're a seasoned pro, aspiring entrepeneur, or passionate hobbyist, our events are tailor-made for tech enthusiasts like you. Bring a laptop, your brightest ideas, and ongoing projects - lets build something together! 
</div> -->

<style>

    .container{
        display: flex;
        justify-content: space-around;
        margin-left: 1.5rem;
        margin-right: 1.5rem;
        margin-top: 1rem;
        margin-bottom: 2rem;

    }

    .about-us-divider{
        background-image: url('./images/about.png') ;
        background-size: cover;
        height: 10em;
        background-position: center;
    
    }

    .about-us-heading{
        font-family: "Bungee";
        margin-right: 1.5em;
        text-align: end;
        font-size: 2.5em;

    }
    .about-us-text{
        background-color: #04010535;
        margin-left: 2em;
        margin-right: 2em;
        font-size: 1.2em;  
        display: flex;
        justify-content: center;   
    }



</style>