<template>
  <div id="app">
    <transition name="animate" enter-active-class="animated bounceInRight" leave-active-class="animated bounceOutRight">
    <router-view/>
    </transition>
  </div>
</template>

<style lang="scss">
@import './styles/main.scss';
</style>
