<template>
  <div class="Bar">
    <h2>
      Bar
    </h2>
    <p>
      Bar - also a fatty.
    </p>
  </div>
</template>

<script>
import bigLibrary2 from '../helpers/big-library-2';

export default {
  name: 'Bar',
  data() {
    return {
      anything: bigLibrary2(),
    };
  },
};
</script>

<style lang="scss">

</style>
