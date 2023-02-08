<template>
  <button @click="openGitHubProfile">View My GitHub Profile</button>
</template>

<script setup>
const openGitHubProfile = () => {
  window.open("https://github.com/shomalikhashayar");
};
</script>
<style>
button {
  font-family: "Rubik", sans-serif;
}
</style>
