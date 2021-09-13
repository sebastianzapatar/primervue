<template>
  <div class="hello">
    <h1>{{mensaje}}</h1>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      mensaje:'hello world'
    }
  }
}
</script>


