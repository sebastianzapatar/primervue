<template>
    <div>
        <h1>Soy el componente Principal</h1>
        <h2>{{nombre}}</h2><br/>
        <input type="text"
        v-model="nombre" />
    </div>    
</template>
<script>
 export default{
     name:"Principal",
     data(){
         return{
             nombre:'',
             edad:0
         }
         
     }
 }
</script>
