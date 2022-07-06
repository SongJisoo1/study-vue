<template>
  <div>
    <div>
      <input type="radio" id="html" value="HTML" v-model="favoriteLang" />
      <label for="html">HTML</label>
    </div>
    <div>
      <input type="radio" id="css" value="CSS" v-model="favoriteLang" />
      <label for="css">CSS</label>
    </div>
    <div>
      <input type="radio" id="js" value="JS" v-model="favoriteLang" />
      <label for="js">JS</label>
    </div>
    <div>{{ favoriteLang }}</div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      favoriteLang: ''
    }
  },
  created() {},
  mounted() {},
  methods: {}
}
</script>
