<template>
  <v-container>
    <ChildPage :id="Number(1)" :state="Number(1)" />
    <draggable v-model="myArray" @start="drag=true" @end="drag=false" group="people">
      <div v-for="element in myArray" :key="element.id">
        {{ element.name }}
      </div>
    </draggable>
  </v-container>
</template>

<script>
import draggable from 'vuedraggable'
import ChildPage from '@/components/ChildPage.vue'

export default {
  components: {
    ChildPage,
    draggable
  },
  data () {
    return {
      myArray: [
        {
          id: 1,
          name: 'java'
        },
        {
          id: 2,
          name: 'python'
        },
        {
          id: 3,
          name: 'php'
        },
        {
          id: 4,
          name: 'javascript'
        }
      ]
    }
  }
}
</script>
