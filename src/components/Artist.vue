<template lang="pug">
  li.artist 
    h2: a(v-bind:href="artist1.url" target="_blank")  {{ artist1.name }}
    img(v-bind:src="artist1.image[2]['#text']")
</template>

<script>

export default {
  name: 'artist',
  props: ['artist1']
  }

</script>

<style lang="stylus" scoped>
li.artist
  display block
  margin 10px 0
</style>
