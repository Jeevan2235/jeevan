<template>
  <div>
    <sidebar />
    <card />
    
  </div>
</template>

<script>
import Card from "~/components/card.vue";
import sidebar from "~/components/sidebar.vue";
export default {
  components: { sidebar, Card,  },
};
</script>

<style>
</style>