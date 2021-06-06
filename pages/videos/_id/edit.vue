<template>
  <div>
    <h1>Editing {{ video.id }}</h1>
    <nuxt-link :to="`/videos/${video.id}/`">
      Back
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: ['video']
}
</script>

<style lang="scss" scoped>

</style>
