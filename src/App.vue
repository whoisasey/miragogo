<template>
<First />
<Second />
<Third />
</template>

<script>
import First from './components/First.vue'
import Second from './components/Second.vue'
import Third from './components/Third.vue'
export default {
  name: 'App',
  components: {
    First,
    Second,
    Third
  },
  data() {
    return {}
  },
  mounted() {
    // via https://codepen.io/anikey99/pen/azmYQY
    $(document).ready(function () {
	$('#nav').localScroll(800);
	
	//.parallax(xPosition, speedFactor, outerHeight) options:
	//xPosition - Horizontal position of the element
	//inertia - speed to move relative to vertical scroll. Example: 0.1 is one tenth the speed of scrolling, 2 is twice the speed of scrolling
	//outerHeight (true/false) - Whether or not jQuery should use it's outerHeight option to determine when a section is in the viewport
	$('#intro').parallax("50%", 0.1);
	$('#second').parallax("50%", 0.1);
	$('.bg').parallax("50%", 0.4);
	$('#third').parallax("50%", 0.3);

})
  }
}
</script>

<style >
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.float-left {
  float: left;
  margin: 0 0 0 20px;
}

.float-right {
  float: right;
  margin: 0 20px 0 0;
}

.center {
  font-size: 2.5em;
  padding: 80px 0 0 0;
  text-align: center;
}

#nav {
  list-style: none;
  position: fixed;
  right: 20px;
}

#nav li {
  margin: 0 0 15px 0;
}

#header,
#intro,
#second {
  width: 100%;
}

.story {
  margin: 0 auto;
  min-width: 980px;
  overflow: auto;
  width: 980px;
}

.story .float-left,
.story .float-right {
  padding: 100px 0 0 0;
  position: relative;
  width: 350px;
}

</style>
