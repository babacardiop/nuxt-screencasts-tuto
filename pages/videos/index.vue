<template>
  <div>
    <h1>Videos</h1>
    <div v-for="video in videos" :key="video.id">
      <nuxt-link :to="`/videos/${video.id}`">
        {{ video.name }}
      </nuxt-link>
    </div>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  data () {
    return {
      videos: [{
        id: '1',
        name: 'Intro to NuxtJS'
      },
      {
        id: '2',
        name: 'Intro to VueJS'
      },
      {
        id: '3',
        name: 'Advanced Techniques for Library X'
      }
      ]
    }
  }
}

</script>

<style lang="scss" scoped>

</style>
