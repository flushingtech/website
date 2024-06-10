<script>
    import Logo from './Logo.svelte';
    import LandingImage from './LandingImage.svelte';
</script>

<div class="container mx-6 my-4">
    <Logo></Logo>
    <LandingImage></LandingImage>
</div>

<section class="about-us-divider">
    <h1 class="about-us-heading text-4xl text-right mr-6 text-white">
        What does this group do?
    </h1>
    <p class="about-us-text bg-opacity-20 p-4 text-xl text-center text-white">
        We hold freeform, self-organized hackathons where creativity knows no bounds. Whether you're a seasoned pro, aspiring entrepreneur, or passionate hobbyist, our events are tailor-made for tech enthusiasts like you. Bring a laptop, your brightest ideas, and ongoing projects - let's build something together! 
    </p>
</section>


<style>
    .container {
        display: flex;
        justify-content: space-around;
    }

    .about-us-divider {
        background-image: url('../routes/images/about.png');
        min-height: 10em; 
        background-position: center;
        padding: 1em; 
        object-fit: cover;
        margin-bottom: 2em;
    }

    .about-us-heading {
        font-family: "Bungee";
    }
</style>
