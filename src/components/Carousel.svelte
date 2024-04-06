<script>
  let currentIndex = 0;
  let projects = [];

  // Fetch project data from projects.json on component mount
  import projectsData from '../projects.json';

  // Map the projectsData to include image URLs in the projects array
  projects = projectsData.map(project => ({
    ...project,
    image_URL: `${project.image_URL}` // Update path to match your image directory
  }));

  function next() {
    currentIndex = (currentIndex + 1) % projects.length;
  }

  function prev() {
    currentIndex = (currentIndex - 1 + projects.length) % projects.length;
  }
</script>

<div class="carousel">
  <button on:click={prev} class="carousel-control left-0">&#8249;</button>
  <img src={projects[currentIndex].image_URL} alt={projects[currentIndex].title} class="w-full">
  <button on:click={next} class="carousel-control right-0">&#8250;</button>
</div>

<style>
  .carousel {
    position: relative;
    width: 100%;
    overflow: hidden;
  }

  .carousel-control {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(255, 255, 255, 0.5);
    padding: 0.5rem;
    border: none;
    cursor: pointer;
    z-index: 10;
  }

  .carousel-control.left-0 {
    left: 0;
  }

  .carousel-control.right-0 {
    right: 0;
  }
</style>
