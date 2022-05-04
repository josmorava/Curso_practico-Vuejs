<template>
  <Layout>
    <template #header>
      <Header />
    </template>

    <template #resume>
      <Resume />
    </template>

    <template #movements>
      <Movements />
    </template>
  </Layout>
</template>

<script>
import Layout from "./LayoutC.vue";
import Header from "./HeaderC.vue";
import Resume from "./resume/IndexC.vue";
import Movements from "./MovementsC.vue";

export default {
  components: {
    Layout,
    Header,
    Resume,
    Movements,
  },
};
</script>
