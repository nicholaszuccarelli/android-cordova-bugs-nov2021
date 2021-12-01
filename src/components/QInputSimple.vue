<template>
  <q-input
    v-model="value"
    dense
    autogrow
    outlined
    label="Enter a value"
  />
</template>

<script>
export default {
  data () {
    return {
      value: ''
    }
  }
}
</script>
