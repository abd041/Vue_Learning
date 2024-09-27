<template>
  <h6>hello world</h6>
  <HelloWorld msg="hello world" />
  <h6>{{ name }}</h6>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
export default {
  name: "App",
  data() {
    return {
      name: "Muhammad Abdullah Rauf"
    }
  },
  components: {
    HelloWorld,
  }
}
</script>
