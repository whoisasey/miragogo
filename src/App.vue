<template>
  <div class="paraContainer">

  <First />
  <Second />
  <Third />

  </div>    
</template>

<script>
import First from './components/First'
import Second from './components/Second'
import Third from './components/Third'

export default {
  name: 'App',
  components: {
First, Second, Third
  },
  data(){
    return {}
  },

}
</script>

<style >
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: whitesmoke;
}

.stretcher{
    display: flex;
    flex-wrap: nowrap;
    flex-direction: row;
    width: 5000px;
}

.stretchDiv{
    height: 100px;
    width: 400px;
    border: solid;

}
/* this is the body divs */
h1{
    text-align: center;
    font-size: 36px;
    margin: 100px;
    font-size: 60px;
    letter-spacing: 2px;
}
h2{
    text-align: center;
    font-size: 36px;
    font-size: 60px;
    letter-spacing: 2px;
    
}
.paraContainer{
    display: flex;
    flex-wrap: nowrap;
    flex-direction: row;
    width: 5000px;
    height: calc(100vh - 2em);

}

.para{
   	display: flex;
	justify-content: center;
	align-items: center;
  	width: 20%;
}

.parainner {

   	display: flex;
	justify-content: center;
	align-items: center;
}

body::-webkit-scrollbar {
    width: 1em;
}
 
body::-webkit-scrollbar-track {
    -webkit-box-shadow: inset 2px rgba(0,0,0,0.3);
    box-shadow: inset 2px rgba(0,0,0,0.3) ;
}
 
body::-webkit-scrollbar-thumb {
  background-color: rgba(0,255,2);
  box-shadow: 15px 5px 4px grey;
  border-radius: 10%;
  border:solid black 2px;
  outline: 20px solid ;
}

</style>
