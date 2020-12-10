<template>
    <div>
        <h5>Dados do Servidor</h5>
        <app-servidor-estado></app-servidor-estado>
        <app-servidor-temperatura></app-servidor-temperatura>
        <hr>
    </div>
</template>

<script>

    import ServidorEstado from './ServidorEstado';
    import ServidorTemperatura from './ServidorTemperatura';

    export default{
        components: {
            'app-servidor-estado' : ServidorEstado,
            'app-servidor-temperatura' : ServidorTemperatura
        }
    }
</script>