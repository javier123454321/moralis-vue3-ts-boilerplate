<template>
  <div class="container p-3">
    <h1>Hello World</h1>
    <p>This is the home page</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "@vue/runtime-core";
import { useStore } from "vuex";

export default defineComponent({

  setup() {
    const store = useStore();
    return {
      user: store.state.User.user,
    };
  },
});
</script>
