<script>
import questions from '../data/questions'
export default {
    name:'AppMain',
    data(){
        return{
            questions
        }

    }
}
</script>

<template>
<main>
    <div v-for="(item,index) in questions " :key="index" class="domanda">
        {{item.domanda}}
    </div>
    <div v-for="(ris,index) in questions" :key="index" class="risposte">
        <button class="risposta">
        {{ris.risposta}}
        </button>
  
         <button class="risposta">
            {{ris.risposta}}
        </button>
         <button class="risposta">
            {{ris.risposta}}
            
        </button>
         <button class="risposta">
            {{ris.risposta}}
            
        </button>

    </div>

</main>
  
</template>



<style lang="scss" scoped>
main{
    background-color:rgb(17 9 58);
    height: 100vh;
}
.domanda{
    width: 20%;
    border-radius: 150px;
    color: white;
    border: 2px solid white;
    margin: 0 auto;
    text-align: center;
    padding: 5px;
}
.risposte{
    margin-top: 30px;
    display: flex;
    flex-wrap: wrap;
    width: 500px;
    margin: 0 auto;
}
.risposta{
    margin: 20px;
    border-radius: 150px;
    padding: 5px;
    width: 200px;
    color: white;
    background-color:rgb(17 9 58);
    border: 2px solid white;
    cursor: pointer;
}
.risposta:hover{
    background-color: rgba(203, 201, 201, 0.795);
}
.risposta:active{
    transform: translateY(4px);

}

//media queries

 @media screen and (max-width:420px) {
    .risposte{
        width: 100%;
        justify-content: center;
    }
    .domanda{
        width: 80%;
    }
 }




</style>