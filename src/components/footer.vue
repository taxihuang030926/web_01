<template>
  <div class="footer">
    <body>
		<link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
  		<footer class="footer">
  	 		<div class="sec">
  	 			<div class="row">
  	 				<div class="footer-col">
  	 					<router-link to="/about"><h4>About</h4></router-link>
  	 				</div>
  	 				<div class="footer-col">
  	 					<router-link to="/project"><h4>Project</h4></router-link>
  	 				</div>
  	 				<div class="footer-col">
  	 					<router-link to="/news"><h4>News</h4></router-link>
  	 				</div>
        			<div class="footer-col">
            			<router-link to="/blog"><h4>Blog</h4></router-link>
  	 				</div>
        			<div class="footer-col">
            			<router-link to="/contact"><h4>Contact</h4></router-link>
  	 				</div>
  	 				<div class="footer-col" style="width:20%;">
  	 					<p style="font-size: 20px; color: #000; font-weight: 500; margin-bottom: 35px; position: relative;">Follow Me</p>
  	 					<div class="social-links">
  	 						<a href="https://www.facebook.com/timmy.haung.1"><i class="fab fa-facebook-f"></i></a>
  	 						<a href="https://www.youtube.com/channel/UC2lmuzvi5b-9nYQ6qjbtN6A"><i class="fab fa-youtube"></i></a>
  	 						<a href="https://www.instagram.com/timmyhaung/"><i class="fab fa-instagram"></i></a>
  	 						<a href="https://github.com/taxihuang030926"><i class="fab fa-github"></i></a>
  	 					</div>
  	 				</div>
  	 			</div>
				<p style="margin-bottom:0px; font-size:10px; justify-content:center;">All rights reserved.</p>
  	 		</div>
  	</footer>

	</body>
  </div>
</template>

<script>
export default {
    name : "Footer"
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/footer.scss"
</style>