<template>
<h2 v-if="num === 0 ">The number is zero</h2>
<h2 v-else>The number is not zero</h2>

<div v-for="(name, index) in fullnames" :key="index">{{ name.name }}

  <h4 v-for="(move , index) in name.movies" :key="index">
          {{move }}
  </h4>
</div>


</template>

<script>

export default {
  name: "App",
  data() {
    return {
     num:1,
     names:["name 1" , "name 2" , "name 3" , "name 4"],
     fullnames :[{
      name:"hello",
      movies:["a1" , "a2" , "a3"]
     },
     {
      name:"hello",
      movies:["a1" , "a2" , "a3"]
     }
    
    ]
    }
  },
}
</script>

<style scoped>
.Hello{
  background: rebeccapurple;
}
.Helloh{
  background: red;
}
</style>