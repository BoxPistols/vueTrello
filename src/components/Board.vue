<template>
  <div>
    <header>my Trello</header>
    <main>
      <p class="info-line">All: 0 tasks</p>
      <ListAdd />
    </main>
  </div>
</template>

<script>
import ListAdd from './ListAdd.vue'

export default {
  name: '',
  data: () => ({}),
  components: {
    ListAdd,
  },
}
</script>

<style lang="scss" scoped="scoped"></style>
