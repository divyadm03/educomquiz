<template>
  <div class="quiz">
    <h1>This is an quiz page</h1>
     
    <!--<div v-for-key="data in myJson"> {{data}}</div> -->
  </div>
</template>
 <script>
       import JSON from 'C:/Users/Divya/Desktop/trial/ast/src/jsonn/data1.json'
 
      export default{
          data(){
              return{
                  myJson: JSON 
              }
          }
      }
</script>
