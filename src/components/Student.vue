<template>
<div>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
   <h1 class="text-center">Student</h1>
  <table class="table table-striped">
    <thead>
      <tr>
        <th>Name</th> <th>Surname</th> <th>Age</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="item in talabalar" :key="item">
        <td>{{item.name}}</td><td>{{item.surname}}</td><td>{{item.age}}</td>
      </tr>
    </tbody>
  </table>
</div>

</template>

<script>
export default {
  name:"Student",
  data(){
    return{
      talabalar:[
        {
          name:'Abdullo',
          age:10,
          surname:'Tolibov'
        },
        {
          name:'Rasullo',
          age:15,
          surname:'Elnazar'
        },
        {
          name:'Alisher',
          age:14,
          surname:'Rasulov'
        },
        {
          name:'Tolibjon',
          age:23,
          surname:'Tolibov'
        },
        {
          name:'Ibodullo',
          age:20,
          surname:'Hoshimov'
        }
      ]
    }
  }
}
</script>