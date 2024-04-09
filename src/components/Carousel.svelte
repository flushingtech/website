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


  <div class="wrapper">

    <div class="left">
      <button on:click={prev} class="carousel-control text-white hover:text-green-500 rounded-full">
        <span class="material-symbols-outlined text-8xl">chevron_left</span>
      </button>
    </div>

    <div class="box2">
      <a>
        <img class="carousel-image " src={projectsData[currentIndex].image_URL} alt={projectsData[currentIndex].title} >
      </a>
    </div>

    <div class="right">
      <button on:click={next} class="carousel-control text-white hover:text-green-500 rounded-full">
        <span class="material-symbols-outlined text-8xl">chevron_right</span>
      </button> 
    </div>

    <div class="box4">
      <div class="title">
        {projectsData[currentIndex].title}
      </div>
      <div class="description">
        {projectsData[currentIndex].description}
      </div>
    </div>
  </div>


  
<!-- when icon is clicked (active state) it will get slightly darker -->
<style>
  /* .carousel-control span.material-symbols-outlined:active {
    filter: brightness(70%);
  } */

  .wrapper {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-template-rows: auto;
}

.left {
  grid-column-start: 1;
  grid-column-end: 2;
  grid-row-start: 2;
  grid-row-end: 3;
  justify-self: center;
}

.box2 {
  grid-column-start: 2;
  grid-column-end: 5;
  grid-row-start: 1;
  grid-row-end: 4;
}

.right{
  grid-column-start: 5;
  grid-column-end: 6;
  grid-row-start: 2;
  grid-row-end: 3;
  justify-self: center;

}
.box4{
  grid-column-start: 2;
  grid-column-end: 5;
  grid-row-start: 4;
  grid-row-end: 5;
}

</style>