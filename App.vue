<template>
  <view class="container">
    <text class="text-color-primary">My Vue Native Apps</text>
    <text-input
      :style="{height: 40, width: 120 ,borderColor: 'gray', borderWidth: 1}"
      v-model="message"
      />
    <button class="btn" v-bind:title="message" v-bind:on-press="handleBtnPress"/>
    </view>
</template>
 
<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: black;
}
.btn{
  background-color: #0d47a1;
}
</style>
<script>
export default {
  data: function() {
    return {
      message: "Hello Vue"
    };
  },
  methods: {
    handleBtnPress: function() {
      alert('Btn Press');
    }
  }
};
</script>