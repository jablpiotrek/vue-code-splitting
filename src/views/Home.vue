<template>
  <div class="home">
    <button class="home__show-foo" @click="showFoo">
      Show Foo!
    </button>
    <foo v-if="isFooVisible" />
  </div>
</template>

<script>


export default {
  name: 'home',
  data() {
    return {
      isFooVisible: false,
    };
  },
  components: {
    Foo: () => import(/* webpackChunkName: "Foo" */ '../components/Foo.vue'),
  },
  methods: {
    showFoo() {
      this.isFooVisible = true;
    },
  },
};
</script>

<style lang="scss">
.home {
  margin-top: 20px;
  border: 1px solid #898989;
  padding: 10px;
  border-radius: 2px;

  &__show-foo {
    padding: 10px;
    margin: 4px;
    width: 100px;
    text-align: center;
    border: 1px solid #898989;
    font-size: 16px;
  }
}
</style>
