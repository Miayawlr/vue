<template lang="pug">
div(:class="$style.buttons")
  zi-button(size="small" :icon="display") action
  zi-button(:iconRight="github") github
  zi-button(size="big" :icon="database") database
</template>

<script>
import display from '@zeit-ui/vue-icons/packages/display'
import github from '@zeit-ui/vue-icons/packages/github'
import database from '@zeit-ui/vue-icons/packages/database'

export default {
  name: 'ex-button-icon',

  components: { display, github, database },

  data: () => ({
    display,
    github,
    database,
  }),
}
</script>

<style module lang="stylus">
.buttons
  >button
    display block
    margin-bottom 8px
</style>
