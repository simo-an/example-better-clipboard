<template>
  <div id="app">
    <button class="alt" @click="open()">查看剪贴板内容</button>
    <router-view></router-view>
  </div>
</template>

<script>
import { betterClipboard } from 'better-clipboard'

// const betterClipboard = require('better-clipboard').betterClipboard

export default {
  name: 'example-better-clipboard',
  methods: {
    open () {
      console.warn(betterClipboard.readFilePathList())
    }
  }
}
</script>

<style>
  /* CSS */
</style>
