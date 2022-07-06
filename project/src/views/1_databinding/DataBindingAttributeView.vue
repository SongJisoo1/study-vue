<template>
  <div>
    <input type="text" v-bind:value="userId" readonly />
    <input type="text" :value="userId" readonly />
    <br />
    <img :src="imgSrc" alt="" style="width: 100px; height: auto" />
    <input type="search" v-model="txt1" />
    <button :disabled="txt1 === ''">serch</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'jisoo97',
      imgSrc: '',
      txt1: ''
    }
  },
  created() {},
  mounted() {},
  methods: {}
}
</script>
