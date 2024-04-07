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

<div class="carousel-container relative flex justify-center my-4">
  <div class="carousel relative max-w-screen-md">
    <div class="flex items-center justify-center"> 
      <button on:click={prev} class="carousel-control mr-2 p-2 text-white hover:text-green-500 rounded-full">
        <span class="material-symbols-outlined text-7xl">chevron_left</span>
      </button>
      <img src={projectsData[currentIndex].image_URL} alt={projectsData[currentIndex].title} class="carousel-image">
      <button on:click={next} class="carousel-control ml-2 p-2 text-white hover:text-green-500 rounded-full">
        <span class="material-symbols-outlined text-7xl">chevron_right</span>
      </button>
    </div>
    <div class="carousel-title text-center mt-2"> 
      {projectsData[currentIndex].title}
    </div>
  </div>
</div>
