<template>
    <div>
        <h1>Soy el componente Principal</h1>
        <h2>{{nombre}}</h2><br/>
        <input type="text"
        v-model="nombre" /><br/>
        <div v-for="persona in estudiantes" :key="persona.id">
            <persona :persona="persona"/>
        </div>
    </div>    
</template>
<script>
import Persona from './Persona.vue'
 export default{
  components: { Persona },
     name:"Principal",
     data(){
         return{
             nombre:'',
             estudiantes:[
                {id:1,nombre:'Lorena',apellido:'Lopez',edad:19},
                {id:2,nombre:'Juan David',apellido:'SantaMaria',edad:22},
                {id:3,nombre:'Juan Pablo',apellido:'Herrera',edad:18},
                {id:4,nombre:'Alexi',apellido:'Lopez',edad:19},
                ]
         }
         
     }
 }
</script>
