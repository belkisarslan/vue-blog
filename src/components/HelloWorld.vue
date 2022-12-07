<template>
  <div class="hello">
    <Container/>
  </div>
</template>

<script>
import Container from './Container.vue';

export default {
    name: "HelloWorld",
    components: { Container }
}
</script>


<style scoped>
h3 {
  margin: 40px 0 0;
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
