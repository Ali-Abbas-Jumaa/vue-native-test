<template>
  <view class="container">
    <text class="text-color-primary">My Vue Native App, Hello world</text>
     <button v-bind:title="message" v-bind:on-press="handleBtnPress"/>
  </view>
</template>
<script>
export default {
  data: function() {
    return {
      message: "Hello world"
    };
  },
  methods: {
    handleBtnPress: function() {
      alert('Btn Press');
    }
  }
};
</script>
<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
