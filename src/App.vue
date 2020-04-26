<template>
  <div>  
    <h1>{{ title + i+ times}}</h1>
    <button @click="iAmClicked()">I dare you to click!</button>
  </div>
</template>
 
<script>
    export default {
       
        data() {
            return {
                title: 'Well done ! You have cliked : ',
                i : 0 ,
                times :" times",
            }
        },
        methods: {

        
            iAmClicked() {
                this.i +=1;
                this.title = "Good job, you have cliked : ";
                this.times =" times";
            },

           
        }
    };
</script>