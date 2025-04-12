<template>
  <div class="toggle-map">
    <button @click="show = !show">
      {{ show ? 'Hide' : 'Show' }} Map
    </button>
    <div v-if="show" class="map-container">
      <iframe
        src="/_icon.html"
        width="100%"
        height="500"
        style="border: none;"
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ToggleMap',
  data() {
    return {
      show: false
    }
  }
}
</script>

<style scoped>
.toggle-map {
  margin-top: 20px;
}
.map-container {
  margin-top: 10px;
  width: 100%;
  height: 500px;
}
</style>
