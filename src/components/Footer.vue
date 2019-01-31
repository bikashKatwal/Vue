<template>
  <div>
    <footer>{{ footerContent }}</footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      footerContent: "Copyright @Online Web Tutor Developers 2018"
    };
  }
};
</script>

<style scoped>
footer {
  background: #3f51b5f2;
  color: white;
  padding: 7px;
  text-align: center;
}
</style>
