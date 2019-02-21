<template>
<div id="app">
	<nav>
	<router-link to="/">Home</router-link>
	<router-link to="/about">About</router-link>
	</nav>
	<img alt="Vue logo" src="./assets/logo.png">
	<router-view/>
</div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Test from './components/Test.vue'

// export default {
//   name: 'app',
//   components: {
//     HelloWorld
//   }
// }


</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat');
#app{
text-align : center;
font-family: 'montserrat', 'sans-serif';

}
body {
background-color: #EEEEEE;
font-family: 'Montserrat', sans-serif;
display: grid;
grid-template-rows: auto;
justify-items: center;
padding-top: 50px;
}

nav {
padding: 20px 0 20px 0;
}

nav a {
padding: 10px;
text-decoration: none; 
background: #ffffff;
border-radius: 2px;
color : blue;
font-weight: bold;
margin-right: 15px;
}

</style>
