<template>
  <h6>hello world</h6>
  <HelloWorld msg="hello world" />
  <h6>{{ name }}</h6>
  <h5 v-bind:id="headingId">Heading</h5>
  <button v-bind:disabled="isDisabled">Button</button>
  <h5 v-bind:class="{
    'Hello':isDisabled,
    'Helloh':isnotDisabled
  }">Button</h5>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
export default {
  name: "App",
  data() {
    return {
      name: "Muhammad Abdullah Rauf",
      headingId:"Heading Id",
      isDisabled:false,
      isnotDisabled:false,
    }
  },
  components: {
    HelloWorld,
  }
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