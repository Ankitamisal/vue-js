<template>
<!-- <h1>Name.....!{{Name}}</h1>
<h1>Email.....!{{email}}</h1>
<h1>Mobile ....!{{Mobile}}</h1>
<h1>Mobile ....!{{Mobile==8888}}</h1>
<h1>company....!{{getName('geoSpoc')}}</h1> -->

<!-- <h1 v-on:mousemove="getConsole()">Home</h1>
<button v-on:click="getData()">Click Me!</button> -->
<h2>pass data to child Components</h2>
<childPage name="GeoSpoc" :user="user" :getData="getData" />

<!-- <h2>{{count}}</h2> -->
</template>

<script>
import childPage from './childPage.vue'
export default {
    name: "homePage",
    components: {
        childPage
    },
    data() {
        return {
            // count: 0,
            user: {
                name: 'ankita',
                email: 'anaw@g.com'
            }
        };
    },
    methods: {
        getData() {
            // this.count = this.count + 1;
            console.log("parent function called")

        },
        /*   getConsole() {
              console.warn("function called");
          } */
    },

}
=======
<!-- <h1 v-on:mousemove="getConsole()">home</h1>
<button v-on:click="getData()">Click Me!</button>
<button v-on:dblclick="getData()">Click Me!</button> -->
<h2>two way binding</h2>
<input type="text" v-model="count">
<h3>{{count}}</h3>

  <p>A list of names that boys: {{namesThatRhyme.join(', ')}}</p>
<label>
  <input type="checkbox" value="Daniel" v-model="namesThatRhyme"/>
  Daniel
</label>
<label>
  <input type="checkbox" value="Nathaniel" v-model="namesThatRhyme"/>
  Nathaniel
</label>
<label>
  <input type="checkbox" value="john" v-model="namesThatRhyme"/>
  john
</label>

<p>How are you feeling today?</p>
  <label>
    <input type="radio" value="great" v-model="howAreYouFeeling" />
    great
  </label>
  <label>
    <input type="radio" value="wonderful" v-model="howAreYouFeeling" />
    wonderful
  </label>


<h3>get input field</h3>
<input type="text" placeholder="enter email" v-model="email">
<input type="password" placeholder="enter password" v-model="password">
<button  v-on:click="inputData()" type="button">Get Values</button>


<h2 v-if="show">If -else Condition</h2>
<button  v-on:click="show=ture">show</button>
</template>

<script>

export default {
    name:'homePage',
    
  data() {
    return {
      howAreYouFeeling: "great",
      namesThatRhyme: [],   
      show:true,
      email:null,
      password:null
    };
  },
    
    //  data()
    // {
    //      return{
    //         count:10
    //      }
    // },
    methods:{ 
      inputData()
      {
       console.log("values:",this.email,this.password) 
      }  
    
 /* getData()
{
  this.count=this.count+1;
},
getConsole()
{
    // alert(a)
     console.log("function called")
} */
 }
} 

</script>

<style scoped>
h2 {
    color: orange;
}

</style>
=======
input {
    margin: 10px;
    padding: 5px;
}
h2,p{
    color: red;
}
h3{
    color: green;
}
</style>
