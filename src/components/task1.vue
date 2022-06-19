<template>
    <div>
        <p v-if="n1 + n2 < 10" :class = "{selected:n1 + n2 < 10}">Мало</p>
        <p v-else-if="n1 + n2 >= 10 && n1 + n2 <= 30" :class = "{selected1:n1 + n2 >= 10 && n1 + n2 <= 30}">Нормально</p>
        <p v-else :class = "{selected:n1 + n2 > 30}">Много</p>
    </div>
</template>

<script>
export default {
    name: 'task1',
    mounted(){
        this.n1 = +prompt('Напишите число'),
        this.n2 = +prompt('Напишите число')
    },

    data(){
        return{
            n1: '',
            n2: '',
        }
    }
}
</script>

<style scoped>
    .selected{
        background-color: orange;
    }

    .selected1{
        background-color: green;
    }
</style>