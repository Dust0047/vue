<template>
  <h1>{{ title }}</h1>
  <input type="text" ref="name">
  <button @click="handleClick"> click it </button>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      title: 'my first vue projekt'
    }
  },
methods: {
  handleClick() {  
    console.log(this.$refs.name)

  }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
