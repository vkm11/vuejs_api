<template>
<h1>Call API</h1>
<p v-for ="item in list" :key="item" >
{{item.id}} --- {{item.email}} --- {{item.first_name}}
</p>
</template>

<script>
import axios from 'axios';
export default {
   name: "App",
    data()
    {
        return{
            list:[]
        }
    },
    async mounted()
    {
        let result = await axios.get("https://reqres.in/api/users?page=1");
        console.log("Api data",result.data.data);
        this.list =result.data.data;
    }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
