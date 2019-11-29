<template>
  <v-container>
    <ChildPage :id="Number(1)" :state="Number(1)" />
  </v-container>
</template>

<script>
import ChildPage from '@/components/ChildPage.vue'
export default {
  components: {
    ChildPage
  }
}
</script>
