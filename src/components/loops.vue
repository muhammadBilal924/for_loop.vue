<template>
    <div>
   <h1>For Loop in vue js</h1>
   <table border="1px">
       <tr>
           <td>id</td>
           <td>name</td>
           <td>email</td>
       </tr>
       <tr v-for="user in users" :key="user.id">
           <td>{{user.id}}</td>
           <td>{{user.name}}</td>
           <td>{{user.email}}</td>
       </tr>
   </table>
    </div>
</template>

<script>
    export default {
     name:"loop",
     props:{
      data:String,
      msg:String   
     },data()
     {
         return{
             users:[
             {id:1,name:'M.Bilal',email:'M.bilal@test.com'},
             {id:2,name:'M.Abdullah',email:'M.Abdullah@test.com'},
             {id:3,name:'M.Numan',email:'M.Numan@test.com'},
             {id:4,name:'M.Sufyan',email:'M.Sufyan@test.com'},
             {id:5,name:'M.Zain',email:'M.Zain@test.com'},
             ]
             
         }
     }   
    }
</script>
