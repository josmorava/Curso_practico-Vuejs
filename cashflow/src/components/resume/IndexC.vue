<template>
  <main>
    <p>{{ dateFunc }}</p>
    <h1>{{ amountVisual }}</h1>
  </main>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
    },
    date: {
      type: String,
      default: null,
    },
    totalAmount: {
      type: Number,
    },
    amount: {
      type: Number,
      default: null,
    },
  },
  computed: {
    amountVisual() {
      //Dibuja el un valor entre las dos opciones
      return this.amount !== null ? this.amount : this.totalAmount;
    },
    dateFunc() {
      return this.label !== null ? this.label : this.date;
    },
  },
};
</script>

<style scoped>
main {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
}
h1,
p {
  margin: 0;
  text-align: center;
}
h1 {
  margin-top: 0;
  color: #2ecc71;
}
.grapihic {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  padding: 48px 24px;
  box-sizing: border-box;
}
</style>
