<template>
    <div>
        <p>Estado do servidor: {{estado}}</p>
        <div>
            <button @click="desligar">Desligar o Servidor</button>
        </div>
    </div>
</template>

<script>
export default {
    data: function(){
        return {
            estado: "Ligado"
        }
    },
    methods: {        
        desligar() {
            this.estado = "Desligador"
        },
    },
}
</script>