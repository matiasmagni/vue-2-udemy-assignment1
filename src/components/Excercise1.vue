<template>
  <div>
    <!-- 1) Fill the <p> below with your Name and Age - using Interpolation -->
    <p>VueJS is pretty cool - {{name}}</p>
    <!-- 2) Output your age, multiplied by 3 -->
    <p>Age (x3): {{age}}</p>
    <!-- 3) Call a function to output a random float between 0 and 1 (Math.random()) -->
    <p>Random Number between 0 and 1: {{ getRandomNum() }}</p>
    <!-- 4) Search any image on Google and output it here by binding the "src" attribute -->
    <div>
        <img v-bind:src="image" alt="Google's image" />
    </div>
    <!-- 5) Pre-Populate this input with your name (set the "value" attribute) -->
    <div>
        <input type="text" v-bind:value="name" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Excercise1',
  data () {
    return {
      name: 'Matías J. Magni',
      age: 31 * 3,
      image: 'https://ciesbizblog.files.wordpress.com/2013/12/internetexplorersucks_88340a_3358046.jpg'
    }
  },
  methods: {
    getRandomNum () {
      return Math.random()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
