<template>
  <h4>{{msg}}</h4>
  <div v-html="channel"></div>
</template>

<script>
export default{
  name:"HelloWorld",
  data(){
    return(
      {
         channel:"<b>hello this is channel</b>"
      }
     
    )

  },
  props:{
    msg:String,
    
  }
}
</script>
