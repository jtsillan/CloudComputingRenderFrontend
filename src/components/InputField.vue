<script setup>
import Button from 'primevue/button';
import InputText from 'primevue/inputtext';
</script>
<template>
    <header>
        <div>
            <InputText class="item" v-model="value3" type="text" size="large" placeholder="Write"/>
        </div>
        <div>
            <Button class="item" type="button" label="GO" severity="success"></Button>
        </div>
    </header>
</template>

<style scoped>
header {
  display: flex;
  /*place-items: flex-start;*/
  flex-wrap: wrap;
  position: relative;
  text-align: center;
  justify-content: center; /* Centers horizontally */
  align-items: center; /* Centers vertically */
}

.item {
  margin-top: 2rem;
}

</style>