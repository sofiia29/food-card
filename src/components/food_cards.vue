<template>
   <div>
       <h1>Featured products</h1>
       <img src="src/assets/images/Rectangle 16.svg">

       <div class="card">
           <div class="space_betw">
               <div class="sale">Sale</div>
               <div class="mark">
                   <!-- <img></img> -->
                   <p>4.7</p>
               </div>
           </div>
            <!-- <img></img> -->
           <div class="txt">
               <p>Vegetable</p>
               <h5>Broccoli</h5>
               <div class="price">
                   <p class="crossed">20$</p>
                   <p id="green">15$</p>
               </div>
           </div>
           <button>Add to cart</button>
       </div>
    </div> 
</template>

<script>
export default {
    name:'food_cards',
    data(){
        return{

        }
    }
}
</script>

<style scoped>
    .card{
        padding: 24px;
        width: 323px;
        box-shadow: 0px 2px 20px rgba(116, 141, 84, 0.2);
        border-radius: 10px;
    }
    .space_betw{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .sale{
        background-color:#8BD32E;
        color: white;
        padding: 4px 16px;
        border-radius: 37px;
        font-size: 14px;
    }

    .mark{
        border: 1px solid #D9D9D9;
        border-radius: 37px;
        color: #B6B6B6;
        font-size: 14px;
    }
    .mark p{
        margin: 0;
        padding: 4px 10px;
    }

    .txt{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-bottom: 32px;
    }

    .txt p{
        margin: 0;
        color: #B6B6B6;
        font-size: 16px;
    }

    .txt h5{
        margin: 0;
        margin-top: 6px;
        margin-bottom: 10px;
        color: #1F201F;
        font-size: 18px;
        font-weight: 700px;
    }

    .price{
        display: flex;
        flex-direction: row;
        gap: 10px;
    }

    .crossed{
        text-decoration: line-through;
    }

    #green{
        color: #8BD32E;
    }

    button{
        background-color: #FDA624;
        width: 100%;
        padding: 12px 24px;
        border: none;
        border-radius: 47px;
        font-size: 16px;
        color: white;
    }
</style>