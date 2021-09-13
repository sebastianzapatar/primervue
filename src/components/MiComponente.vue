<template>
  <div id="miComponente">
      <h1>Esto es el componente que yo cree</h1>
      <h2>{{subtitulo}}</h2>
      {{/*
      Este un comentario de JavaScript
      */}}
      <!-- Este es un comentario de html-->
      <p v-if="edad>=18">
          Eres mayor de edad
      </p>
      <p v-else-if="edad==17">
          casi te falta poco
      </p>
      <p v-else>
          Eres menor de edad no se puede ir a beber
      </p>
      <div v-for="estudiante in estudiantes" :key="estudiante.id">
          <persona :persona="estudiante"/>
      </div>
  </div>
  
</template>

<script>

import Persona from './Persona.vue'
export default {

    name:"MiComponente",
    components:{
        Persona
       
    },
    data(){
        return{
            subtitulo:'Soy el profesor y tengo hambre',
            mensaje:"Soy el mensaje del componente hijo",
            edad:16,
            sueldo:10,
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
