<template>
  <button @click="openGitHubProfile">{{ textWillShowOnButton }}</button>
</template>

<!-- script setup -->
<script setup>
const props = defineProps({
  textWillShowOnButton: {
    type: String,
    default: "View My GitHub Profile",
  },
});
const openGitHubProfile = () => {
  window.open("https://github.com/shomalikhashayar");
};
</script>

<!-- composition api -->
<!--
<script>
export default {
  setup() {
    const openGitHubProfile = () => {
      window.open("https://github.com/shomalikhashayar");
    };

    return { openGitHubProfile };
  },
  props: {
    textWillShowOnButton: {
      type: String,
      default: "View My GitHub Profile",
    },
  },
};
</script>
-->

<style>
button {
  font-family: "Rubik", sans-serif;
}
</style>
