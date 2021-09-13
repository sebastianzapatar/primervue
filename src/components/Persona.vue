<template>
    <div>
        <strong>Nombre: </strong>{{persona.nombre}} <br/>
        <strong>Apellido: </strong>{{persona.apellido}}<br/>
        <strong>Edad: </strong> {{persona.edad}}
        <p v-if="persona.edad>=20"> Mandelo a trabajar </p>
        <p v-else>Siga estudiando</p>
    </div>   
</template>
<script>
    export default{
        name:"Pelicula",
        props:['persona']
    }
</script>
