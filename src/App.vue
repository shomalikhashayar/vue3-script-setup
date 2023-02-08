<template>
  <h1>My name is {{ name }}, I'm {{ age }} years old.</h1>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const name = ref("Khashayar Shomali");
const age = ref(22);
</script>

<!-- script setup with return
<script>
import { ref } from "@vue/reactivity";

export default {
  setup() {
    const name = ref("Khashayar Shomali");
    const age = ref(22);

    return {
      name,
      age,
    };
  },
};
</script>
-->
