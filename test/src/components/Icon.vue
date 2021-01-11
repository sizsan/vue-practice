<template>
    <q-icon :color="color" :name="name"/>
</template>
<script>
export default {
  props: {
    color: {
      type: String,
      default: 'red'
    },
    name: {
      type: String,
      required: true
    }
  }
}
</script>
