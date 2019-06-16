<template>
  <div class="home">
    <button @click="showFoo">
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
