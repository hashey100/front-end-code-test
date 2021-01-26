<template>
  <div>
    <ul>
      <li v-for="article in articles"
      :key="article.title">
        {{ article.title }}
      </li>
    </ul>
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  computed: {
    ...mapState('articles', ['articles']),
  }
}
</script>
