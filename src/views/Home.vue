<template>
  <div class="home">
    <CardUser />
  </div>
</template>

<script>
// @ is an alias to /src
import CardUser from "@/components/CardUser.vue";

export default {
  name: "Home",
  components: {
    CardUser
  }
};
</script>
