<template>
  <layout-c>
    <template #header>
      <header-c />
    </template>
  </layout-c>
</template>

<script>
import LayoutC from "./LayoutC.vue";
import HeaderC from "./HeaderC.vue";

export default {
  components: {
    LayoutC,
    HeaderC,
  },
};
</script>
