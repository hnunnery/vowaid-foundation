<template>
  <div class="contact">
    <Contactform/>
  </div>
</template>

<script>
import Contactform from "@/components/Contactform";

export default {
  name: "contact",
  components: {
    Contactform
  },
  data() {
    return {};
  },
  metaInfo: {
    titleTemplate: "%s | Contact Us"
  }
};
</script>

<style lang="scss" scoped>
</style>
