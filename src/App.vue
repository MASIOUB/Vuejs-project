<template>
  <div id="app">
    <NavbarContent />
    <div class="content">
      you clicked on this {{ counter }} times
      <br />
      <div class="btn">
        <button @click="counter++">click</button>
      </div>
    </div>
    <FooterContent />
    <tests />

    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

// export default {
//   name: 'App',
//   components: {
//     HelloWorld
//   }
// }
import NavbarContent from "./components/navbarContent.vue";
import FooterContent from "./components/footer.vue";

export default {
  name: "App",
  components: {
    NavbarContent,
    FooterContent,
  },
  data: function () {
    return {
      counter: 0,
    };
  },
};

// export default Navbar{
//   // name: navbar,
//   data(){
//     return{

//     }
//   }
// }
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
.content {
  min-height: 80vh;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
}

.content button {
  width: 100px;
  justify-self: center;
}
</style>
