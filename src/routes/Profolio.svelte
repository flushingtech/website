<div class="card-container">
    <div class="card" style="width: 18rem;">  
        <div class="card-body">
          <h5 class="card-title">Card title</h5>
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
        <img src="https://placehold.co/600x400/png" class="card-img-top" alt="...">
      </div>
</div>

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