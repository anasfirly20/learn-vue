<template>
    <p v-if="age < 25">This message is only shown to ages above 25</p>
    <p v-else>You are above 25 years old!</p>
    
   <p>{{msg}}</p>
</template>

<script>
 export default {
    name: 'Greeting',
    props: ['age'],
    data(){
      return {
        msg: 'Hello world'
      }
    }
  }
</script>

<style scoped lang="scss">
p:hover {
    color: darken(#cc4444, 15%)
}
</style>