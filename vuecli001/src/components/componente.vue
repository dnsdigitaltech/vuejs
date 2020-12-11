<template>
    <div>
        <p>Componete Child</p>
        <p>{{valor1}}</p>
    </div>
</template>
<script>
export default {
    props: {
        valor1:{
            type: String,
            default: 'Davi Bernardo'
        }
    }
}
</script>