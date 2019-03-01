<template>
  <div class="home">
    <Mission/>
    <Team/>
  </div>
</template>

<script>
import Mission from "@/components/Mission";
import Team from "@/components/Team";

export default {
  name: "index",
  components: {
    Mission,
    Team
  }
};
</script>