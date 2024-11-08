<template>
  <div class="container">
    <h3 class="title" v-if="title" :id="id">{{ title }}</h3>
    <div class="content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "CustomSection",
  props: {
    title: {
      type: String,
      required: false
    },
    id: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.title {
  font-size: 22px;
}

.content {
  background-color: var(--color-background-light);
  border-radius: 7px;
  padding: 1rem 2.5rem;
}

.container {
  width: 90%;
  margin: 2rem auto;
}
</style>