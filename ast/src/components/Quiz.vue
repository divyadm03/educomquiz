<template>
  <div class="quiz">
    <h1>This is an quiz page</h1>
    <p>{{ question }}</p>
     
    
  </div>
</template>
 <script>
 export default{ 
   name: 'Quiz',
   data(){
     return{
     question:""
     }
   },
   mounted(){
     this.$http.get('http://localhost:8000/api/questions').then(result =>{
                 this.question=result.question;
     },error =>{
       console.error(error);
     });
   }
  }
  
  
 </script>
