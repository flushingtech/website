<script>
  let currentIndex = 0;

  // Fetch project data from projects.json on component mount
  import projectsData from '../projects.json';

  function next() {
    currentIndex === projectsData.length - 1 ? currentIndex = 0 : currentIndex += 1
  }

  function prev() {
    currentIndex === 0 ? currentIndex = projectsData.length - 1 : currentIndex -= 1
  }
</script>

<div class="carousel-heading text-5xl mb-6 text-center bg-black bg-opacity-80" style="font-family: 'Bungee Shade', sans-serif; color:#baf553ff">
  Our Work
</div>

<div class="carousel-container flex items-center justify-center">
  <div class = "left ml-20 mr-4 ">
    <button on:click={prev} class="carousel-control text-white hover:text-green-500 rounded-full">
      <span class="material-symbols-outlined text-8xl">chevron_left</span>
    </button>
  </div>

  <div class="middle flex-col max-w-6xl">
      <a>
        <img class="carousel-image " src={projectsData[currentIndex].image_URL} alt={projectsData[currentIndex].title} >
      </a>
      
      <div class = "caption bg-black bg-opacity-50 mb-4">
        <div class="project-title text-left mt-2 text-2xl"> 
          {projectsData[currentIndex].title}
        </div>
        <div class="description text-lg">
          {projectsData[currentIndex].description}
        </div>
        <div class="team text-sm">
          Team: {projectsData[currentIndex].team.join('; ')}
        
    
        </div>

      </div>

  </div>

  <div class = "right mr-20 ml-4 ">
    <button on:click={next} class="carousel-control text-white hover:text-green-500 rounded-full">
      <span class="material-symbols-outlined text-8xl">chevron_right</span>
    </button>
  </div>


</div>

<!-- when icon is clicked (active state) it will get slightly darker -->
<style>
  .carousel-control span.material-symbols-outlined:active {
    filter: brightness(70%);
  }
</style>