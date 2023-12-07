<template>
  <div class="wrapper">
  <div class="main-container">
    <div class="container-one">
      <div class="profile">
        <img src="../assets/profile.png" alt="" />
        <h1>Favour A. Uzochukwu</h1>
        <p>Front-End Developer</p>
      </div>

      <div class="social-links">
          <div class="links">
            <a v-bind:href="gitLink">
							<img src="../assets/github.png" alt="">
							<h2>GitHub</h2></a>
          </div>
          <div class="links">
            <a v-bind:href="linkedinLink">
							<img src="../assets/linkedin.png" alt="" />
							<h2>LinkedIn</h2></a>
          </div>
          <div class="links">
            <a v-bind:href="twitterLink">
							<img src="../assets/twitter.png" alt="" />
							<h2>Twitter</h2>
						</a>
          </div>
          <div class="links">
            <a v-bind:href="instagramLink">
							<img src="../assets/instagram.png" alt="" />
							<h2>Instagram</h2>
						</a>
          </div>
      </div>
    </div>
    <div class="container-two">
      <div class="about-me">
        <h1>About Me</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit rerum
          minima facilis fuga non nam veniam quisquam architecto, tempore,
          labore at. Adipisci reiciendis labore sint rerum quod dolorum deserunt
          quia?
        </p>
      </div>
      <div class="technology-section">
        <h1>Technologies</h1>
        <div class="logos">
          <img src="../assets/html.png" alt="" />
          <img src="../assets/css.png" alt="" />
          <img src="../assets/js.png" alt="" />
          <img src="../assets/vuejs.png" alt="" />
        </div>
      </div>

      <div class="button-container">
        <div class="projects-button">
          <a href="">My Projects</a>
        </div>

        <div  class="projects-button">
          <a href="">My Resume</a>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
	data() {
		return {
			gitLink: 'https://github.com/Avvyyy/',
			twitterLink: 'https://twitter.com/Avvy_ta/',
			instagramLink: 'https://instagram.com/cod3Gurl/',
			linkedinLink: 'https://www.linkedin.com/in/favour-uzochukwu/'
		}
	},
};
</script>

<style scoped>

body{
	margin: 0px;
	padding: 0px;
}

img {
  width: 20px;
}

.wrapper{
  display: flex;
  justify-content: center;
}

.main-container {
  display: flex;
  flex-direction: row;
	background-color: #A0D4FF;
	border-radius: 25px;
  width: 60%;
}

.container-one{
	background-color:#1292EE;
	width: 40%;
	padding: 2.5%;
	border-radius: 25px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
}

.profile img{
	height: 5rem;
	width: 5rem;
	border: 50%;
}

.links a{
	text-decoration: none;
	color: #2c3e50;
	font-size: 10px;
}

.links img{
	height: 2rem;
	width: 2rem;
}
.container-two{
	width: 60%;
	margin: 2.5%;
}

.about-me{
	text-align: left;
}


.logos {
  display: flex;
  gap: 10px;
  align-items: center;
  justify-content: center;
}

.logos img{
	height: 2.5rem;
	width: 2.5rem;
}

.button-container{
	margin: 5%;
	display: flex;
	flex-direction: row;
	justify-content: center;
	align-items: center;
}

.projects-button{
	background-color: #005CA4;
	margin: 5px;
	padding: 5px;
	border-radius: 15px;
}
.projects-button a{
	text-decoration: none;
	color: #fff;
}

@media only screen and (max-width: 950px){
  .main-container{
    width: 95%;
  }
}
</style>
