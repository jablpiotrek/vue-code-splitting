<template>
  <div class="app">
    <h1 class="app__heading">Vue code splitting</h1>
    <div class="app__navigation">
      <router-link class="app__navigation-item" to="/">Home</router-link>
      <router-link class="app__navigation-item" to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
.app {
  @import url('https://fonts.googleapis.com/css?family=Fira+Sans&display=swap');

  &__heading {
    text-align: center;
    width: 100%;
  }

  &__navigation {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  &__navigation-item {
    padding: 10px;
    margin: 4px;
    width: 100px;
    text-align: center;
    border: 1px solid #898989;
    border-radius: 2px;
    text-decoration: none;
    color: black;
    &:hover,
    &:focus {
      border-color: black;
    }
  }

  h1,h2,p,a,button {
    font-family: 'Fira Sans', sans-serif;
  }
}
</style>
