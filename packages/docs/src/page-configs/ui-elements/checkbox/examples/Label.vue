<template>
  <div class="d-flex flex-direction-column">
    <va-checkbox class="mb-4" v-model="value" :label="label" />
    <va-checkbox class="mb-4" v-model="value" :label="longLabel" />
    <va-checkbox v-model="value" :label="leftLabel" left-label />
  </div>
</template>

<script>
export default {
  data () {
    return {
      value: true,
      label: 'Label',
      longLabel:
          'This label is pretty long, but still perfectly fits the layout...',
      leftLabel: 'Left label',
    }
  },
}
</script>
