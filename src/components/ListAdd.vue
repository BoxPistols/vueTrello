<template>
  <div>
    <form class="addlist" @submit.prevent="addList">
      <input
        v-model="title"
        type="text"
        class="text-input"
        placeholder="Add new list"
      />
      <button type="submit" class="add-button">
        Add
      </button>
    </form>
  </div>
</template>

<script>
export default {
  name: '',
  data: () => ({
    title: '',
  }),
  methods: {
    addList() {
      this.$store.dispatch('addlist', { title: this.title })
      this.title = ''
    },
  },
}
</script>

<style lang="scss" scoped></style>
