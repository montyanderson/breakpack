<template>
	<div id="app">
		<h1>breakpack</h1>

        <hr>
		<p class="about-1">Based in Bristol, UK and Founded by Niall Shaw in 2021, Breakpack is a music platform for a collection of forward-thinking electronic producers, with the aim of connecting more likeminded individuals across the country from different genres, encouraging collaboration to bring out a new underground sound for electronic music.</p>
        <p class="about-2"> Featuring artists such as short_ghost, Sunbleach, and Spheress.<br>
		<br>
Build by Monty Anderson, Oliver Wilcox, and Oliver Redman.</p>
	  	<div class="releases">
		  	<Release v-for="r in releases" v-bind:release="r"></Release>
	  	</div>
	</div>
</template>

<script>
import Release from './components/Release.vue';

export default {
  name: 'App',
  components: {
	  Release
  },
  data: () => ({
	  releases: [
	  ]
  })
}
</script>

<style>
#app {
	width: 375px;
	min-height: 800px;
	position: absolute;
	transform: translate(-50%, -50%);
	left: 50%;
	top: 400px;
}

h1 {
	position: absolute;
	width: 268px;
	height: 43px;
	left: 52px;
	top: 108px;

	font-family: Rubik Mono One;
	font-style: normal;
	font-weight: normal;
	font-size: 35px;
	line-height: 43px;

	color: #FFFFFF;
}

.about-1 {
	position: absolute;
	width: 319px;
	height: 126px;
	left: 28px;
	top: 181px;

	font-family: Rubik;
	font-style: normal;
	font-weight: normal;
	font-size: 12px;
	line-height: 14px;
	text-align: justify;

	color: #FFFFFF;
}

.about-2 {
	position: absolute;
	width: 319px;
	height: 70px;
	left: 28px;
	top: 305px;

	font-family: Rubik;
	font-style: normal;
	font-weight: normal;
	font-size: 12px;
	line-height: 14px;
	text-align: justify;

	color: #FFFFFF;
}

hr {
	position: absolute;
	width: 95px;
	height: 0px;
	left: 139px;
	top: 464px;

	border: 2px solid #FFFFFF;
}

.releases {
	position: absolute;
	top: 538px;
	height: auto;
}
</style>
