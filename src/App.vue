<template>
  <div>
    <h1>Welcome to Vue JS Module</h1>
    <p>{{ firstName }} {{ lastName }}</p>
    <div>
      <button @click="changeSurname">Change Surname</button>
    </div>
    <div>
      <h2>Attribute binding</h2>
      <h2>{{ msg }}</h2>
      <input type="text" v-model="msg">
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      firstName: 'Lerato',
      lastName: 'Peter',
      msg: 'Hello class 1'
    }
  },
  components: {},
  methods: {
    changeSurname() {
      this.lastName = "Mukanya"
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
