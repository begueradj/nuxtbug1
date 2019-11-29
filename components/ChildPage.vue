<template>
  <div>
    <ul>
      <li>State. {{ state }}</li>
      <li>ID: {{ id }} </li>
    </ul>
    <div />
  </div>
</template>

<script>
export default {
  name: 'ChildPage',
  props: {
    state: {
      type: Number,
      default: null
    },
    id: {
      type: Number,
      default: null
    }
  }
}
</script>
