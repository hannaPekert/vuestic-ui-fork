<template>
  <docs-content :config="configComputed" />
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component'
import DocsContent from '../../components/DocsContent.vue'
import fileUploadConfig
  from '../../page-configs/ui-elements/file-upload/page-config'

@Options({
  name: 'DocsFileUpload',
  components: { DocsContent },
})
export default class FileUpload extends Vue {
  get configComputed () {
    return fileUploadConfig
  }
}
</script>
