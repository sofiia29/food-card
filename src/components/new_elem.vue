<template>
   <div>
       <p v-if="age > 14">Доступ разрешен</p>
       
    </div> 
</template>

<script>

export default{
    name:'new_elem',
    mounted(){
        this.age = +prompt("How old are you?")
    },
    data() {
        return{
          age: '',  
        }
        
    }
}
</script>

<style scoped>
 
</style>
