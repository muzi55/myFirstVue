<template>
  <h1>뷰 학습</h1>
  <div>
    <h2>카운터 만들기</h2>
    <img alt="Vue logo" src="./assets/logo.png" />
    <p>{{ count }}</p>
    <button v-on:click="increase">증가</button>
    <button @click="decrease">감소</button>
  </div>
  <hr />

  <div>
    <h2>배열 반복하기/ 반복문</h2>

    <!-- <div>카레</div>
    <div>마파두부</div>
    <div>돈까스</div> -->

    <!-- <div>{{ food[0] }}</div>
    <div>{{ food[1] }}</div>
    <div>{{ food[2] }}</div> -->

    <!-- <div v-for="(a, i) in food" :key="i">{{ a }}</div> -->
    <!-- 뷰에서 반복학습 -->
    <div v-for="a in food" :key="a">{{ a }}</div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      count: 0,
      food: ["카레", "마파두부", "돈까스"],
    };
  },
  methods: {
    increase() {
      this.count++;
    },
    decrease() {
      this.count--;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
