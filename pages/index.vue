<template>
  <div class="root">
    <appHeader></appHeader>
    <h1>Overskrift</h1>
    <appFooter></appFooter>
  </div>
</template>

<script>
import appHeader from '~/components/appHeader'
import appFooter from '~/components/appFooter'
export default {
  components: {
    appHeader,
    appFooter
  }
};
</script>

<style scoped>
h1 {
  color: black;
}

</style>
