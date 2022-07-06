<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="myFunction">click</button>
    <button @click="changeDate">change</button>
    <hr />
    <input type="text" v-model="num1" /> +
    <input type="text" v-model="num2" /> =
    <span>{{ num1 + num2 }}</span>
    <hr />
    <input type="text" v-model.number="num3" /> +
    <input type="text" v-model.number="num4" /> =
    <span>{{ num3 + num4 }}</span>
  </div>
</template>
<script>
export default {
  data() {
    return {
      userId: 'jisoosong97',
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0
    }
  },
  created() {},
  mounted() {},
  methods: {
    myFunction() {
      console.log(this.userId)
    },
    changeDate() {
      this.userId = 'Jeremy'
    }
  }
}
</script>
