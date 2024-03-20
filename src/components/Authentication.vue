<template>
    <form class="add-form">
     <div>
         <div class="form-control">
         <label>Authentication</label>
         <input type="text" name="text" placeholder="Client ID" />
         </div>
         <div class="form-control">
         <label>Description</label>
         <input type="text" name="text" placeholder="Description" />
         </div>
       
     </div>
 </form>
 
 </template>
 
 <script>
 export default{
     name: "Authentication"
 }
 </script>
 
 <style scoped>
 .add-form {
   margin-bottom: 40px;
   flex: 1;
 }
 
 .form-control {
   margin: 20px 0;
 }
 
 .form-control label {
   display: block;
 }
 
 .form-control input {
   width: 100%;
   height: 40px;
   margin: 5px;
   padding: 3px 7px;
   font-size: 17px;
 }
 
 .form-control-check {
   display: flex;
   align-items: center;
   justify-content: space-between;
 }
 
 .form-control-check label {
   flex: 1;
 }
 
 .form-control-check input {
   flex: 2;
   height: 20px;
 }
 
 
 </style>