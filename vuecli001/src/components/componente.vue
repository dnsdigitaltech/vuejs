<template>
    <div>
        <p>(Component.vue) Nome: {{meunome}}</p>
        <button @click="alterar()">Alterar</button>
    </div>
</template>
<script>
export default {
    props: ['meunome'],
    methods: {
        alterar(){
            this.meunome = "Bernardo"
            this.$emit('nomeAlterado', this.meunome)
        }
    },
}
</script>