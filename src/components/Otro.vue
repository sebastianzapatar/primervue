<template >
    <div>
        <h3>{{Mensaje}}</h3>
        <h4>{{texto}}</h4>
    </div>
</template>
<script>
export default{
    name:"MiComponente",
    props:['texto'],
    data(){
        return{
            Mensaje:'Soy el componente hijo'
        }
        
    }
    }
</script>
