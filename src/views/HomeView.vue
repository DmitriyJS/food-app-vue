<template>
  <div class="home">
    <button @click="showLog({ a: `asdf`, b: 22 })">Home</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

type aaa = {
  a: string;
  b: number;
};

interface test extends aaa {
  с?: any;
}

export default defineComponent({
  name: "HomeView",
  components: {},
  methods: {
    showLog(num: test) {
      console.log(num);
    },
  },
});
</script>
