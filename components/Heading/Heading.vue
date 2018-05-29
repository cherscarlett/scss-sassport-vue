<script>
  import Vue from 'vue'

  Vue.component('HeadingTag', {
    render: function (createElement) {
      return createElement(
        this.$parent.$props.level,
        this.$slots.default
      )
    },
  })

  export default {
    props: ['level', 'href', 'size', 'theme']
  }
</script>

<template lang='haml' src='./Heading.haml' />

<style lang='scss'>
  @import './Heading.scss';
</style>
