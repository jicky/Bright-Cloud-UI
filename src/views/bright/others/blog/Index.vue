<template>
  <i-frame
    :src="url"
    @refresh="refresh"
  />
</template>
<script>
import iFrame from '@/components/iFrame'
export default {
  components: { iFrame },
  data() {
    return {
      url: 'https://github.com/JacksonTu'
    }
  },
  methods: {
    refresh(u) {
      this.url = u
    }
  }
}
</script>
