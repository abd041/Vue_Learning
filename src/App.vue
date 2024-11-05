<template>
  <h4>{{ add(1 , 2 ,4) }}</h4>
  <h4>{{ add(8, 5 , 10) }}</h4>
</template>

<script>

export default {
  name: "App",
  data() {
    return {
    }
  },
  methods :{
  add(a,b,c){
    return a + b + c
  }
  }
}
</script>

<style scoped>
</style>