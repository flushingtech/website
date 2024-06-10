<script>
	import pic1 from '../routes/images/Option5.png';
	import pic2 from '../routes/images/Option4.png'
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
img{
	/* width: 400px;
	border-radius: 2px;
	min-width: 200px; */
}
.image-2{
	transform: scaleX(-1);
}

/* Q */
/* how do you make the image responsive (ie - not scrunch up when window size changes?) */

</style>