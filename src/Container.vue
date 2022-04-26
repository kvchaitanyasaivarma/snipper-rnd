<template>
  <div id="container">
    <Card Cardtitle="Sample" Cardtags="Tag1 , Tag2" Cardcode="PGJ1dHRvbiBAY2xpY2s9ImRpc2FibGVkID0gIWRpc2FibGVkIj5Ub2dnbGUgRW5hYmxlPC9idXR0b24+CjxpbnB1dCB0eXBlPSJ0ZXh0IiBpZD0ibmFtZSIgY2xhc3M9ImZvcm0tY29udHJvbCIgbmFtZT0ibmFtZSIgIHYtbW9kZWw9ImZvcm0ubmFtZSIgOmRpc2FibGVkPSJkaXNhYmxlZCI+Cg=="/>
    <Card Cardtitle="Sample" Cardtags="Tag1 , Tag2" Cardcode="sample code goes here"/>
    <Card Cardtitle="Sample" Cardtags="Tag1 , Tag2" Cardcode="sample code goes here"/>
    <Card Cardtitle="Sample" Cardtags="Tag1 , Tag2" Cardcode="sample code goes here"/>
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'Container',
  components: {
    Card
  }
}
</script>

<style>

</style>
