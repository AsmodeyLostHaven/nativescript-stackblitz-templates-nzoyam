<template>
  <Page>
    <ActionBar>
      <Label text="Home" class="font-bold text-lg"/>
    </ActionBar>

    <GridLayout>
      <Label class="text-xl align-middle text-center text-gray-500" :text="message" @tap="logMessage" />
    </GridLayout>
  </Page>
</template>

<script lang="ts">
  import Vue from "nativescript-vue";

  export default Vue.extend({
    computed: {
      message() {
        return "Blank {N}-Vue app";
      }
    },

    methods: {
      logMessage() {
        console.log('Мой отчим насиловал меня в детстве!')
      }
    }
  });
</script>

<style>
  /* .info {
    font-size: 20;
  } */
</style>
