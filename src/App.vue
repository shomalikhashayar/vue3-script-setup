<template>
  <div class="khashayar-picture">
    <a
      href="http://github.com/shomalikhashayar"
      target="_blank"
      rel="noopener noreferrer"
    >
      <img
        src="../src/assets/khashayar.jpeg"
        alt="Khashayar Shomali"
        title="Khashayar Shomali"
    /></a>
  </div>
  <div class="bio">
    <h1 @mouseover="whenMouseOverHeading" @mouseout="whenMouseOutHeading">
      {{ bio }}
    </h1>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const bio = ref("Hello, My name is Khashayar Shomali, I'm 22 years old.");

const whenMouseOverHeading = () => {
  bio.value =
    "I'm a Software Engineer Who developing SPA websites with VUE.js ";
};
const whenMouseOutHeading = () => {
  bio.value = "Hello, My name is Khashayar Shomali, I'm 22 years old.";
};
</script>

<!--
<script>
import { ref } from "@vue/reactivity";

export default {
  setup() {
    const bio = ref("Hello, My name is Khashayar Shomali, I'm 22 years old.");

    const whenMouseOverHeading = () => {
      bio.value =
        "I'm a Software Engineer Who developing SPA websites with VUE.js ";
    };

    const whenMouseOutHeading = () => {
      bio.value = "Hello, My name is Khashayar Shomali, I'm 22 years old.";
    };

    return {
      bio,
      whenMouseOverHeading,
      whenMouseOutHeading,
    };
  },
};
</script>
-->
<style>
@import url("https://fonts.googleapis.com/css2?family=Rubik&display=swap");

body {
  display: flex;
  justify-content: center;
  margin-top: 50px;
  background-color: bisque;
}

.bio {
  height: 100px;
  width: 900px;
  background-color: blanchedalmond;
  border-radius: 9px;
  box-shadow: 0 4px 12px 0 rgba(255, 143, 15, 0.719);
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 12px;
  font-family: "Rubik", sans-serif;
  cursor: pointer;
}

@media screen and (max-width: 600px) {
  body {
    padding-left: 20px;
    padding-right: 20px;
  }
  .bio {
    height: 100px;
    width: 450px;
    font-size: 10px;
  }

  .bio h1 {
    max-width: 400px;
    text-align: center;
    line-height: 30px;
  }
}
.khashayar-picture img {
  border-radius: 50%;
  width: 250px;
  height: 250px;
  border: 4px solid orange;
  box-shadow: 0 4px 12px 0 rgba(255, 143, 15, 0.719);
  cursor: pointer;
}

.khashayar-picture {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 50px;
}
</style>
