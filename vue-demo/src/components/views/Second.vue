<template>
  <div class="second-app">
    {{ msg }}
    <confirm text="注册" @message="getMessage"></confirm>
  </div>
</template>

<script>
import Confirm from "../sub/Confirm";
export default {
  name: "Second",
  components: {
    Confirm,
  },
  data() {
    return {
      msg: "Welcome to SecondApp",
    };
  },
  methods: {
    getMessage(val) {
      alert(val);
    },
  },
};
</script>

<style>
</style>
