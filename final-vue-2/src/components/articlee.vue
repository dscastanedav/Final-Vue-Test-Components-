<template>
    <div>
        <h2 v-bind="$attrs">Article component: {{title}}</h2>
        <h2>Numero e likes: {{likes}}</h2>
        <h2>Ta publicao? : {{isPublished ? 'Yep' : 'Nop'}}</h2>
    </div>
</template>

<script>
    export default {
        name:'article-comp',
        props:{
            title: {
                type: String,
                required: true,
                default: 'Oieeeee te hablo desde la prisiooooon'
            },
            likes: Number,
            isPublished: Boolean
            //existen mas tipos de props
            //array, objecto como el title ahora, date e incluso pueden haber
            //props funciones, ni idea de como sera eso, pero seguro que 
            //se les pasa un parametro en el template de app.vue
            //y lo que se imprime del template del componente.vue debe ser el resultado
            //de evaluar la funcion con ese parametro
        },
        //esta vaina se usa para hacer que los props tenga individualmente su id, y no se lo 
        //pasen por defecto a su contenedor
        inheritAttrs: false
    }
</script>

<style lang="sass" scoped>

</style>