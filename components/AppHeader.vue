<template>
  <header>
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
  </header>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Default Header'
    }
  },
  setup() {
    const description =
      'This is a description coming from the script in the Header component.'
    return {
      description
    }
  }
}
</script>
