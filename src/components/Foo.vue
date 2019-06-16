<template>
  <div class="foo">
    <h2>
      Foo
    </h2>
    <p>
      Foo - the fat component.
    </p>
  </div>
</template>

<script>
import bigLibrary from '../helpers/big-library';

export default {
  name: 'Foo',
  data() {
    return {
      something: bigLibrary(),
    };
  },
};
</script>

<style lang="scss">

</style>
