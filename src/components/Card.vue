<template>
<div id="#tenu">
  <h1 class="text-center">Our Products</h1>
   <div class="row " style="margin-left: 30px">
     <div class="card" v-for="item in Velo" :key="item">
       <div class="col-md-6" >
         <div class="card-header">
           <img :src="item.image" alt="">
         </div>
         <div class="card-body text-center" style="width: 700px">
           <h3>Name: {{item.name}}</h3>
           <h4>Country: {{item.country}}</h4>
           <h5>Age: {{item.age}}</h5>
           <h3>Price:{{price}}$</h3>
           <a class="btn badge-success">Add cart:{{count}}</a>
           <a class="btn btn-danger"  v-on:click="minus">Minus</a>
           <a class="btn btn-primary" v-on:click="plus">
             Plus
           </a>
           <a href="#" style="float: left" class="btn badge-success"><span>Total: {{count*price}}$</span></a>
         </div>
       </div>
     </div>
   </div>
   </div>

</template>
<script>
//  export default(){
//   el:"#tenu",
//
//   data(){
//
//     //    price=[16.59,27.99,27.41,14.92,18.36,31.43,19.74,27.59],
//     count:0
//   },
//   methods:{
//     // price:function(){
//     //     this.price++
//     // },
//     plus:function(){
//       this.count++
//     },
//     minus:function(){
//       if(this.count>0)
//         this.count--
//     }
//   }
// }
export default {
  name:"Card",
  data( ){
    return{
      Velo:[
        {
          name:"WhiteFuture_velo",
          country:"America",
          age:"new",
          image:"https://i.pinimg.com/originals/41/18/20/4118207856865b48b26fb127acbf2472.jpg"
        },
        {
          name:"YellowFuture_moterbiKe",
          country:"Uzbekistan",
          age:"new",
          image:"https://media.zigcdn.com/media/model/2021/Aug/lest-side-view-384309212_600x400.jpg"
        },
        {
          name:"WhiteFuture_velo",
          country:"America",
          age:"new",
          image:"https://techcrunch.com/wp-content/uploads/2020/07/Screen-Shot-2020-07-13-at-11.19.07-AM.jpg?w=600"
        },
        {
          name:"RedFuture_velo",
          country:"Canada",
          age:"new",
          image:"https://cdn.shopify.com/s/files/1/0676/4159/products/ImagesG4i_5_600x.jpg?v=1629764147"
        },
        {
          name:"WhiteFuture_velo",
          country:"Mexico",
          age:"new",
          image:"https://d1wa5qhtul915h.cloudfront.net/app/uploads/2015/04/attachment-001_logistiek-image-BIK5689I01.jpg"
        },
        {
          name:"BlackFuture_velo",
          country:"Italiano",
          age:"new",
          image:"https://cdn.shopify.com/s/files/1/0505/9729/8352/products/Black-ebike-white_066d7ed8-e453-47c6-bd23-0f103f77f872_grande.png?v=1637880883"
        }
      ]
    }
  }

}
</script>