<template>
  <div class="about">
    <bar />
  </div>
</template>
<script>
import Bar from '../components/Bar.vue';

export default {
  name: 'About',
  components: {
    Bar,
  },
};
</script>

<style lang="scss">
.about {
  margin-top: 20px;
  border: 1px solid #898989;
  padding: 10px;
  border-radius: 2px;
}
</style>
