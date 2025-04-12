<template>
  <div class="info">
    <h1>{{ msg }}</h1>
    <p>
      Software Engineer and DevOps enthusiast. 
    </p>
    <h3>Open Source projects</h3>
    <ul>
      <li><a href="https://github.com/LuisFros/image_plane_classifier" target="_blank" rel="noopener">Image Plane Classifier</a></li>
      <li><a href="https://github.com/LuisFros/rails-dockerizado" target="_blank" rel="noopener">Full Stack Rails + Vue on Docker</a></li>
      <li><a href="https://github.com/LuisFros/docker-model-evaluator" target="_blank" rel="noopener">Docker ML Model evaluator</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a v-bind:href="pdfPath" target="_blank">Resume/CV</a></li>
    </ul>
  </div>
</template>

<script>

const pdfPath = "https://es.overleaf.com/download/project/5f89a12f7b67070001d6631e/output/output.pdf?compileGroup=priority"

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return {pdfPath}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
