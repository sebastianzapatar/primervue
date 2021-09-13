<template>
    <div>
        <strong>Nombre: </strong>{{persona.nombre}} <br/>
        <strong>Apellido: </strong>{{persona.apellido}}<br/>
        <strong>Edad: </strong> {{persona.edad}}
    </div>   
</template>
<script>
    export default{
        name:"Pelicula",
        props:['persona']
    }
</script>
