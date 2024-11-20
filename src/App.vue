<script setup>
import TheWelcome from './components/TheWelcome.vue';
import WelcomeSmiley from './components/WelcomeSmiley.vue';
import InputField from './components/InputField.vue';
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/smiley.png" width="125" height="125" />

    <div class="wrapper">
      <WelcomeSmiley msg="Welcome!" />
    </div>
  </header>
  <body>
    <div class="body">
      <InputField></InputField>
    </div>
  </body>
</template>

<style scoped>
header {
  line-height: 1.5;
}


.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
