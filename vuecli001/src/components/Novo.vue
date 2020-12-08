<template>
    <div>
        <p>Olá Mundo! {{nome}} {{apelido}}</p>
    </div>
</template>

<script>
    export default{
        methods:{
            click: function(){

            }
        },
        data:function(){
            return {
                nome: "Davi",
                apelido: "Bernardo"
            }
        }
    }
</script>