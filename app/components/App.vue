<template>
  <Page>
    <ActionBar title="Welcome to NativeScript-Vue!"/>
    <GridLayout columns="*" rows="*">
      <Button class="message" text="test" @tap="test" col="0" row="0"></Button>
    </GridLayout>
  </Page>
</template>

<script >
 import Waa from "./Waa";

export default {
  data() {
    return {
      msg: "Hello World!"
    };
  },
  methods: {
    test() {
      this.$navigateTo(Waa, { clearHistory: true });
    }
  }
};
</script>

<style scoped>
ActionBar {
  background-color: #53ba82;
  color: #ffffff;
}

.message {
  vertical-align: center;
  text-align: center;
  font-size: 20;
  color: #333333;
}
</style>
