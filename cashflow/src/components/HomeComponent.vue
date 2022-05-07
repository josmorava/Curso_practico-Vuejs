<template>
  <Layout>
    <template #header>
      <Header />
    </template>

    <template #resume>
      <Resume
        :label="label"
        :amount="amount"
        :totalAmount="100000"
        :totalLabel="totalLabel"
      >
        <template #graphic> Grapihc </template>

        <template #action> Action </template>
      </Resume>
    </template>

    <template #movements>
      <Movements
        :movements="movements"
      />
    </template>
  </Layout>
</template>

<script>
import Layout from "./LayoutC.vue";
import Header from "./HeaderC.vue";
import Resume from "./resume/IndexC.vue";
import Movements from "./movements/IndexC.vue";

export default {
  components: {
    Layout,
    Header,
    Resume,
    Movements,
  },
  data() {
    return {
      amount: null,
      label: "Ahorro total",
      totalLabel: null,
      movements: [{
        id: 0,
        title: "Movimiento 1",
        description: "bla bla bla bla bla",
        amount: 100,
      }, {
        id: 1,
        title: "Movimiento 2",
        description: "bla bla bla bla bla",
        amount: -100
      }, {
        id: 2,
        title: "Movimiento 3",
        description: "bla bla bla bla bla",
        amount: 230
      }, {
        id: 3,
        title: "Movimiento 4",
        description: "bla bla bla bla bla",
        amount: -200
      }, {
        id: 4,
        title: "Movimiento 5",
        description: "bla bla bla bla bla",
        amount: 500
      }]
    }
  },
};
</script>
