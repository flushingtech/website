<script>
  let currentIndex = 0;

  // Fetch project data from projects.json on component mount
  import projectsData from '../projects.json';


  function next() {
    currentIndex === projectsData.length-1 ? currentIndex = 0 : currentIndex+=1
  }

  function prev() {
    currentIndex === 0 ? currentIndex = projectsData.length-1 : currentIndex-=1
  }
</script>

<div class="carousel-container">
  <div class="carousel">
    <button on:click={prev} class="carousel-control left-0">&#8249;</button>
    <img src={projectsData[currentIndex].image_URL} alt={projectsData[currentIndex].title} class="carousel-image">
    <button on:click={next} class="carousel-control right-0">&#8250;</button>
    <div class="carousel-title">{projectsData[currentIndex].title}</div>
  </div>
</div>

<style>
  .carousel-container {
    max-width: 80%; /* Adjust the maximum width of the carousel */
    margin: 0 auto; /* Center align the carousel */
  }

  .carousel {
    position: relative;
    width: 100%;
    overflow: hidden;
    border: 2px solid #000; /* Optional: Add a border around the carousel */
    border-radius: 8px; /* Optional: Add border radius for a rounded look */
    text-align: center; /* Center align carousel content */
  }

  .carousel-image {
    width: 100%; /* Ensure the image fills the carousel container */
    height: auto; /* Maintain aspect ratio */
    display: block; /* Remove any default image spacing */
  }

  .carousel-control {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    padding: 0.5rem;
    border: none;
    cursor: pointer;
    z-index: 10;
    color: #000; /* Set button color to black */
    background-color: #fff; /* Set button background to white */
  }

  .carousel-control.left-0 {
    left: 0;
  }

  .carousel-control.right-0 {
    right: 0;
  }

  .carousel-title {
    padding: 1rem;
    font-size: 1.5rem;
    font-weight: bold;
    color: #fff; /* Set title color to white */
  }
</style>
