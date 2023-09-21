<template>
  <div class="home">
    <wysiwyg-editor></wysiwyg-editor>
  </div>
</template>

<script>
// @ is an alias to /src
import WysiwygEditor from '@/components/WysiwygEditor.vue'

export default {
  name: 'HomeView',
  components: {
    WysiwygEditor
  }
}
</script>
