<script>
	import pic1 from '../images/man.png';
	import pic2 from '../images/woman.png'
</script>
<div class= "landing-img-container">
	<img src={pic1} alt="graphic art depicting man using laptop and working on a mobile application."/>
	<img class="image-2" src={pic2} alt="graphic art depicting woman using some kind of organizational/planning tool. She seems to be collaborating with the man from the previous image."/>
	
</div>

<style>
	.landing-img-container{
		display:flex;
		width:65%;
	}

.image-2{
	transform: scaleX(-1);
}

</style>