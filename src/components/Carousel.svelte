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


  <div class="grid grid-cols-5 gap-4">

    <div class="left col-start-1 col-span-1 row-start-2 row-span-1 justify-self-center">
      <button on:click={prev} class="carousel-control text-white hover:text-green-500 rounded-full">
        <span class="material-symbols-outlined text-8xl">chevron_left</span>
      </button>
    </div>

    <div class="image col-start-2 col-span-3 row-start-1 row-span-3">
      <a href = {projectsData[currentIndex].project_link} target="_blank">
        <img class="carousel-image " src={projectsData[currentIndex].image_URL} alt={projectsData[currentIndex].title} >
      </a>
    </div>

    <div class="right col-start-5 col-span-1 row-start-2 row-span-1 justify-self-center">
      <button on:click={next} class="carousel-control text-white hover:text-green-500 rounded-full">
        <span class="material-symbols-outlined text-8xl">chevron_right</span>
      </button> 
    </div>

    <div class="caption col-start-2 col-span-3 row-start-4">
      <div class="title text-2xl">
        {projectsData[currentIndex].title}
      </div>
      <div class="description text-lg mb-6">
        {projectsData[currentIndex].description}
      </div>
    </div>
  </div>


  
<!-- when icon is clicked (active state) it will get slightly darker -->
<style>
  .carousel-control span.material-symbols-outlined:active {
    filter: brightness(70%);
  }
</style>