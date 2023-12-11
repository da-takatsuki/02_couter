<template>
  <div class="box">
    <div id="title">Vue Counter</div>
    <p id="count">{{ count }}</p>
    <div class="_button">
      <button id="_increment_button" @click="increment">+</button>
      <button id="_decrement_button" @click="decrement">-</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
  },
};
</script>

<style scoped>
.box {
  width: 300px;
  height: 400px;
  background-color: #fff;
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.button {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

#_increment_button {
  border-radius: 50%;
  width: 70px;
  height: 70px;
  background-color: #1c5cd0;
  border-color: #1c5cd0;
  color: #fff;
  margin: 0px 20px;
  font-size: 24px;
}

#_decrement_button {
  border-radius: 50%;
  width: 70px;
  height: 70px;
  background-color: #fff;
  border-color: #1c5cd0;
  color: #1c5cd0;
  margin: 0px 20px;
  font-size: 24px;
}

#title {
  font-size: 24px;
  font-weight: bold;
  margin: 12px;
  color: #aaa;
}

#count {
  font-size: 48px;
  font-weight: bold;
  margin: 60px 0px;
  color: #1c5cd0;
}
</style>
