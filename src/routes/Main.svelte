<script>
    import Logo from './Logo.svelte';
    import LandingImage from './LandingImage.svelte';
</script>

<div class="container">
    <Logo></Logo>
    <LandingImage></LandingImage>
</div>

<div class="about-us-divider">
    <div class="about-us-heading">
        What does this group do?
    </div>
    <div class="about-us-text">
        We hold freeform, self-organized hackathons where creativity knows no bounds. Whether you're a seasoned pro, aspiring entrepreneur, or passionate hobbyist, our events are tailor-made for tech enthusiasts like you. Bring a laptop, your brightest ideas, and ongoing projects - let's build something together! 
    </div>
</div>

<style>
    .container {
        display: flex;
        justify-content: space-around;
        margin-left: 1.5rem;
        margin-right: 1.5rem;
        margin-top: 1rem;
        margin-bottom: 2rem;
    }

    .about-us-divider {
        background-image: url('./images/about.png');
        min-height: 10em; /* Changed height to min-height */
        background-position: center;
        padding: 1em; /* Added padding for spacing */
        object-fit: contain;
        
    }

    .about-us-heading {
        font-family: "Bungee";
        margin-right: 1.5em;
        text-align: end;
        font-size: 2.5em;
        color: white; /* Added text color */
    }

    .about-us-text {
        background-color: rgba(4, 1, 5, 0.2); /* Changed opacity */
        margin: 1em; /* Added margin for spacing */
        font-size: 1.2em;  
        text-align: center; /* Centered text */
        color: white; /* Added text color */
    }
</style>
