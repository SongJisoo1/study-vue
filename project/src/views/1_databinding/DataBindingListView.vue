<template>
  <div>
    <div>
      <select name="" id="">
        <option value=""></option>
        <option :value="city.code" :key="city.code" v-for="city in cities">
          {{ city.title }}
        </option>
      </select>
    </div>
    <div>
      <table>
        <thead>
          <tr>
            <th>제품번호</th>
            <th>제품명</th>
            <th>가격</th>
            <th>주문수량</th>
            <th>합계</th>
          </tr>
        </thead>
        <tbody>
          <tr :key="drink.drinkId" v-for="drink in drinkList">
            <td>{{ drink.drinkId }}</td>
            <td>{{ drink.drinkName }}</td>
            <td>{{ drink.price }}</td>
            <td><input type="number" v-model="drink.qty" /></td>
            <td>{{ drink.price * drink.qty }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      cities: [
        { title: '서울', code: '02' },
        { title: '부산', code: '051' },
        { title: '제주', code: '064' }
      ],
      drinkList: [
        {
          drinkId: '1',
          drinkName: '코카콜라',
          price: 700,
          qty: 1
        },
        {
          drinkId: '2',
          drinkName: '코카콜라2',
          price: 700,
          qty: 1
        },
        {
          drinkId: '3',
          drinkName: '코카콜라3',
          price: 700,
          qty: 1
        },
        {
          drinkId: '4',
          drinkName: '코카콜라4',
          price: 700,
          qty: 1
        },
        {
          drinkId: '5',
          drinkName: '코카콜라5',
          price: 700,
          qty: 1
        },
        {
          drinkId: '6',
          drinkName: '코카콜라6',
          price: 700,
          qty: 1
        },
        {
          drinkId: '7',
          drinkName: '코카콜라7',
          price: 700,
          qty: 1
        }
      ]
    }
  },
  created() {},
  mounted() {},
  methods: {}
}
</script>
