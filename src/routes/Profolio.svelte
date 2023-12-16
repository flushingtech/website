<script>
let projects = [{
    "projectName":"Project Name",
    "purpose":"Purpose of the project",
    "technologyUsed":"Technology used to complete project",
    "status":"status of project",
    "url":"url",
    "image":"https://placehold.co/600x400/png",
    "duration":"duration of project",
    "license":"license used"
},{
    "projectName":"Project Name 2",
    "purpose":"Purpose of the project 2",
    "technologyUsed":"Technology used to complete project 2",
    "status":"status of project 2",
    "url":"url 22222",
    "image":"https://placehold.co/600x400/png",
    "duration":"duration of project res lorem ipsum",
    "license":"license used"
}]

</script>
{#each projects as project}
<div class="card-container">
    <div class="card" style="width: 18rem;">
          
        <div class="card-body">
          <h5 class="card-title">{project.projectName}</h5>
          <p class="card-text">{project.purpose}</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
        <img src="{project.image}" class="card-img-top" alt="...">

      </div>
</div>
{/each}
<style>
    .card-container{
        display: flex;
    }
    .card{
        border: 1px solid red;
        display:flex;
        flex:auto;
        justify-content: center;
    }
    .card-title{
        font-size: large;
        font-weight: bold;
        margin-bottom: 20px;
    }
    .card-text{
        margin-bottom: 30px;
    }
    .btn{
        background-color: lightblue ;
        border-radius: 8px;
        padding: 5px;
        margin-bottom: 10px;
    }
</style>